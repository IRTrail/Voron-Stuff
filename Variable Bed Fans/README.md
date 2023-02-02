# Variable Bed Fan Control
###### for people who just need to fuck with things that work well already.
I started with [Andrew Ellis' bed fans control macro](https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/Ellis/Bed_Fans). Then I thought, well, if those four bed fans can cool the bed faster than the heater can heat, wouldn't it be nice to make them change to keep the bed using about 80% of usable power?

So, that's what I did.

This adaptation makes a pretty rudimentary proportional controller for the bed fans. It monitors the heater bed power use, then changes the bed fans speed based on that. If the power use gets high, then the fans slow down to allow the bed to heat up. If the power use is low, then the fans speed up, cooling the bed and necessitating more power use.

### So, what good is that?
Well, I am glad you asked. It's automated, and that in itself should be reason enough for you to install my bug ridden macro on your printer. None of your friends have it, therefore, you're ~~dumber~~ braver than they are.
Also, it maximizes the heat transfered into the chamber, which should give you a few degrees more chanber temp and a bit faster heat soak than the gold standard bed fans macro. But, who really cares about performance when **_its automated_**?

## The parameters:
### power:
The target power useage. On my Voron, keeping 0.4 watts per square centimeter equals out to limiting the bed heater to 60%. I use 55% as a target, to leave a little overhead. Above this target, the fans will start slowing down.
### coeff:
The coefficient applied to the delta between current power usage and target useage, then multiplied by the fast fan speed. The formula looks like this:
Fast fan speed + coefficient * (difference between target and actual power use)
### others:
They're all the same as Ellis' macro and work the same.

## Explaination:
According to those who drink and know things, you should shoot for about 0.4 watts per square centimeter of bed area. This is to avoid tacoing the bed. On my Voron V2.4 that turns out to be 60% maximum power to the bed heater. It's enough to heat the bed up in about 10 minutes. After that, the PWM shown in Mainsail starts tapering off to around ~40%. So, theres 20% of the bed power that is just wasted. It could be used to heat the chamber more quickly and get it hotter in the process. So, we can speed the fans up a little when the power is about 5% less than full (55% in my case). When it's above that, we slow the fans down because the bed needs to stay at the prescribed temperature.

In reality, you could just work on fine tuning the fast fan speed from the original macro and likely never need this one. However, I found that it settles down pretty quickly and works pretty good vs printing for a couple hours and adjusting, then repeating. I originally set the power target to 55% and the fast fans speed to 0.3 since I have four bed fans. With the macro running, the actual fan speed settles down to about 0.36. Then I set the fast fan speed to 0.4 and the fans settled down to about 0.37. So, I think the macro finds an optimal fan speed over all.

That being said, it doesn't ever really stay at the target power use. The PID on the bed drifts quite wildly at times. So, I would recommend the coeff variable be low (0.2-0.5) and your fast bed fan speed be tuned pretty well. If you use coeff=1.0 and the power delta is large enough, it can get into a cycle where it fights its self and then you get a Klipper shutdown because the bed isn't heating correctly.

I would love any feedback. This is still very much a work in progress.