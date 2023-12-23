# G2E and Filametrix
## _Modifications for the G2E to have a Filametrix cutter...and a filament sensor option...or two._  
### Thanks to sundee, jmaurin, jelliebean, and kinematicdigit for suggestions and feedback. Thanks to any of you who have come here and print these parts. You're what it's all about.
These parts are at the conceptual stage currently. If you use them and find issues, please let me know via DM through discord @ silverback_attack. I am still in the process of printing and installing this setup. There will likely be updates.
Also, understand there is no CAD released for the G2 stuff. Reverse engineering it is a total PITA. Ergo, there will likely be some slicer complaints because the stls aren't "water tight."
Use at your own risk. It's not my fault your sister is ugly or your tongue hurts when you lick a 9V battery...or anything else. Just saying.

![Filametrix for G2E](https://github.com/IRTrail/Voron-Stuff/assets/53546870/7d406f1e-ca80-48ee-9c7e-a4754e9f7497)


### _All Licenses are carried over from their respective creators. Read them here:_
https://github.com/sorted01/Filametrix
https://github.com/JaredC01/Galileo2
If not otherwise licensed, the files herein are covered by GPL V3. See LICENSE in this directory.  

## There are now two versions. One is sensored, the other is without sensor. See the respective folders for CAD and STL files.
Unless otherwise stated below, all the build notes from the G2E and Filametrix apply. If you look things over, you should get the idea.

### Filametrix Parts:
This is just the arm which has been modified to not interfere with the G2E motor.  

### G2E Parts:
These are modified from the STLs of the G2E. You'll need to print a front and back. Then put the heatset insert in per the Filametrix Method.  

<details><summary>Instructions for inserting drilled heatset and PTFE tube for non-sensored version</summary>  
  
#### Deviation (non-sensored):
I ended up installing the heatset insert in the front and drilling it out to 4mm with progressively larger drills. I made the drilled hole just about to the location where the extruder gears "point" is. Then I installed a piece of PTFE tube in it, and trimmed it flush.

If you don't want to do that, the CAD is such that the filament path is sized for 1.75mm filament (or at least what the G2E guys thought was a good diameter for 1.75mm filament) all the way to the heatset. Let me know if you use this and how it works.

As an aside, it is an utter PITA to get that PTFE tube in the motor plate. I finally figured out that if you cut a piece a bit long, then put the tubing on a 1.5mm hex driver, the kind that looks like a small screw driver with a *comfortable* handle, you can easily push the tubing in place. Then trim flush.

1. Cut the tube a bit too long:  
![PXL_20231220_142135729](https://github.com/IRTrail/Voron-Stuff/assets/53546870/70fdd213-97e0-4778-836b-e7b3f58f3931)  

2. ***IMPORTANT!*** You'll need to countersink the end of the PTFE tube that goes toward the gears. Otherwise, the flat end of the tip will catch and absolutely NOT feed. Seriously.  
Just use a countersink cutter like you'd find in the woodworking section of the hardware store. Alternatively, if you're into R/C stuff, a body reamer for R/C cars works well.  

3. Fit the tube on a 1.5mm hex driver. In the picture is a Bondhus brand driver. I think I got the set on Amazon for $17 or so. Note that the countersink end goes AWAY from the driver handle.  
![PXL_20231220_142354741](https://github.com/IRTrail/Voron-Stuff/assets/53546870/631eb58b-8c05-4407-b9b2-506ac4c0cc7e)

4. Push the tube in to place. I mean PUSH! It takes a bit of effort, but make sure you get it all the way in. (TWSS)  
![PXL_20231220_142429565](https://github.com/IRTrail/Voron-Stuff/assets/53546870/0e34f2db-9504-40ac-ba4d-af43514da0a3)  
Here's the tube seated in the extruder body:  
![PXL_20231220_142527996](https://github.com/IRTrail/Voron-Stuff/assets/53546870/49bd3322-76a1-4ed9-ab66-ba7b9bd680b4)  

5. Trim the tube flush with the drilled out heat set:  

###### Notes:
I am not entirely sure how much the heat set helps. I *think* it was intended to create a nice hard surface to shear against the blade. However, it seems to work well with the PTFE tube in there. If I get to the point that I print another extruder body, I'll try one without the heatset and a bore sized for the PTFE tube instead.</details>

<details><summary>Notes on the sensored model</summary>  
  
### This is beta-ish. I have printed but used it yet. Give me feedback if you print and use before I do.  

1. There are now two versions of the sensored G2E front plate. One with a sensor below the extruder gears and the "twinsored" one with a sensor above and below the gears. Your choice. Both should roughly follow the below notes.
2. The design uses a 6x3 magnet to act as a roller between the switch and filament path. Other designs use a 7mm ball. I don't have a bunch of those lying around. However, I do have a plethora of 6x3mm magnets. I figure anyone who has built a Voron 2.4 likely has one which escaped under the couch cushion at some point.
3. I didn't put a heat set insert in the extruder exit. Just shove a piece of PTFE in there an it should work OK. Be sure to countersink the end toward the extruder gears to get a smooth filament path. Hint: If you forgot, a 2.5mm bolt will thread into the PTFE and give you something to grip on and extract the tube. DAMHIKIJD.
4. It uses the standard D2F switch called out in the Voron 2.4 Bill of Materials. You'll want the high force one. If it has an F after D2F, its low force and likely won't be as reliable and possibly sense filament where there is none. It might be good to put the roller at a slight angle and use gravity to pull the roller away from the sensor. I'll just put that on my to-do list.  
5. There are holes in the front of the body to accept 2mm socket head sheetmetal screws. There's not a lot of room behind the switch, so if they don't grab in, it's not a big worry. They're just there to hold the switch in place. If you're nervous about it, you could use a 1.5mm drill to deepen the holes behind the switch.  
6. There are supports. I'm sorry, it's the best I could do. They should break away pretty easy if your printer is tuned well. Dig them out with a screwdriver or needle nose pliers. You might need to touch up the overhang a bit if the switch doesn't easily insert. Since you likely have a bunch of the #4 blades for the cutter, they work pretty good for getting rid of small bulges in the switch cavity.  
7. The distance from the lower switch centerline to the top of the nozzle is 68.3 (ish) mm according to CAD for a Rapido (the OG non ultra high flow) hotend. For the upper switch to the lower is 33mm. From the upper switch to the extruder gears is 13.1 (ish) mm. From the gears to the lower switch is 19.9 (ish) mm.  
8. It should fit an SB2040 from Mellow. I don't have a BTT version. I don't plan on a BTT version. If it works with yours that's cool. Send me a note and I'll include it here.</details>
