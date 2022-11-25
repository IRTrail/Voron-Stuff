This is my first tutorial on Github, so bear with me.

Squaring the gantry, like Andrew Ellis' guide, but with a couple twists.
    See: https://github.com/AndrewEllis93/Print-Tuning-Guide

I recently did the GE5C mod (https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/hartk1213/Voron2.4_GE5C) and found that it makes the gantry more rigid in the plane of the gantry. Basically, the stock type spherical joint device allows the corners of the gantry to float around in the X-Y plane. When the GE5C mod is installed, they are locked into position by the solid bolt and Z-rails.

Previously, I had thought my gantry was square. I am a perfectionist after all, and I had spent literally dozens of minutes getting it perfect. So, it was surprizing that it wasn't square.
Not even close.

In the process, I decided to do the pins mod as well (https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/hartk1213/Voron2.4_Trident_Pins_Mod). So, in that I had to take all the A/B joints loose it gave me a really great opportunity to square up the gantry.

I printed off some Z locks (https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/tallman5/z-locks) and proceeded to lock the gantry in place having the A/B joints installed loosely. This allowed the gantry to settle in place at the "perfect" angle and position. With this setup, the Y rails will not move. They are solidly connected to the frame through the Z rails and Z locks. The next step is to check the cross member between the A/B drive joints. Mine was off center. Since I am a perfectionist and all, well, you just can't be having no off center stuff, even if you can't tell by lookin'. So I centered that and tightened down the A/B joints and the front idlers. The front idlers can't really go anywhere, but I had them loose anyway. Now is a good time to make sure the front of the Y rails is flush with the face of the idlers ala the Voron instruction manual.

Once all that was done, then I looked at the X rail. Using a carpenter's square, I checked to ensure it was square to the Y rails. It wasn't (go figure). So, I messed with that a bit until it was slightly better than perfect, which, as we all know, is almost good enough. Then I tightened those down as well. It's worth noting that I had the A/B belts uninstalled at this point. The printer had some 600 hours print time on it, and, well, I needed to place an order with Fabreeko since I hadn't bought anything 3D printer related for nearly an entire day. So, new belts and some other goodies on the way.

Now is a good time to tune the Z belts with a frequency measuring app on your phone. All the Z lengths should be identical so the frequencies should all be able to tune up OK. Alternatively, the Prusa belt tension gauge can be used to set them all equal. (https://www.printables.com/model/46639-tension-meter-for-the-gt2-belts-of-i3-mk3s-or-prus/files) As a final alternative, one could use the resonance of something that constantly vibrates at any given frequency and tune the belts to resonate with that frequency. I'll leave it to your imagination what that could be.

The final step is to adjust the A/B belts. Once again you could use the app, the gauge, or induced resonance, but I had pretty good luck getting one belt "about right" then checking the squareness of the X and Y rails while tensioning the other. Unequal tension will result in a skewed X rail, which isn't OK unless you drive an old FIAT or something. Just be sure to check the X rail squareness again after you tension the belts.

A couple other hints:

    1. There is such a device as a 1/4" hex drive ratchet. It looks like a regular, albeit small, ratchet, but instead of having a 1/4", 3/8", etc. square drive for a socket, it has a 1/4" hex drive so you can drive hex bits with it. You need one. Get a set of 1/4" drive bits as well.

    2. If you're doing the pins mod, some of the idlers might be too tight on the pins. They are, from what I can see online, a "transition" fit. That means they are somewhere between a mild interference fit and a slide fit. Depending on the pin and the idler bearing, it may be too tight. If that happens, I found it helps to chuck the pin up in a drill and use some Mother's or other metal polish on the pin. This reduces the outer diameter by a slight amount and helps the tighter bearing fit...sometimes.

    3. If you don't have a carpenter's square you can make a right triangle with a comapss (thing that draws circles) and a straight edge. Draw the circle as big as you need, draw the diameter through the center point. Now, mark any point on the circle between the diameter points. Connect the three dots. Boom. Now you have a perfect 90º angle. Just be sure to use something not important you can cut the piece out of. Marriage licenses come to mind...

Maybe, some day, in the distant future, I'll figure out how to make this look better and add some pictures or what not. Maybe...