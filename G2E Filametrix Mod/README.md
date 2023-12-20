# G2E and Filametrix
## _Modifications for the G2E to have a Filametrix cutter._
These parts are at the conceptual stage currently. If you use them and find issues, please let me know via DM through discord @ silverback_attack. I am still in the process of printing and installing this setup. There will likely be updates.
Also, understand there is no CAD released for the G2 stuff. Reverse engineering it is a total PITA. Ergo, there will likely be some slicer complaints because the stls aren't "water tight."
Use at your own risk. It's not my fault your sister is ugly or your tongue hurts when you lick a 9V battery...or anything else. Just saying.

![Filametrix for G2E](https://github.com/IRTrail/Voron-Stuff/assets/53546870/7d406f1e-ca80-48ee-9c7e-a4754e9f7497)


### _All Licenses are carried over from their respective creators. Read them here:_
https://github.com/sorted01/Filametrix
https://github.com/JaredC01/Galileo2
If not otherwise licensed, the files herein are covered by GPL V3. See LICENSE in this directory.  

### Filametrix Parts:
This is just the arm which has been modified to not interfere with the G2E motor.  

### G2E Parts:
These are modified from the STLs of the G2E. You'll need to print a front and back. Then put the heatset insert in per the Filametrix Method.  

#### Deviation:
I ended up installing the heatset insert in the front and drilling it out to 4mm with progressively larger drills. I made the drilled hole just about to the location where the extruder gears "point" is. Then I installed a piece of PTFE tube in it, and trimmed it flush.

If you don't want to do that, the CAD is such that the filament path is sized for 1.75mm filament (or at least what the G2E guys thought was a good diameter for 1.75mm filament) all the way to the heatset. Let me know if you use this and how it works.

As an aside, it is an utter PITA to get that PTFE tube in the motor plate. I finally figured out that if you cut a piece a bit long, then put the tubing on a 1.5mm hex driver, the kind that looks like a small screw driver with a *comfortable* handle, you can easily push the tubing in place. Then trim flush.

##### Step 1:  
Cut the tube a bit too long:  
![PXL_20231220_142135729](https://github.com/IRTrail/Voron-Stuff/assets/53546870/70fdd213-97e0-4778-836b-e7b3f58f3931)  

##### Step 2:  
***IMPORTANT!*** You'll need to countersink the end of the PTFE tube that goes twoard the gears. Otherwise, the flat end of the tip will catch and absolutely NOT feed. Seriously.  
Just use a countersink cutter like you'd find in the woodworking section of the hardware store. Alternatively, if you're into R/C stuff, a body reamer for R/C cars works well.  

##### Step 4:  
Fit the tube on a 1.5mm hex driver. In the picture is a Bondhus brand driver. I think I got the set on Amazon for $17 or so.  
![PXL_20231220_142354741](https://github.com/IRTrail/Voron-Stuff/assets/53546870/631eb58b-8c05-4407-b9b2-506ac4c0cc7e)  

##### Step 5:
Push the tube in to place. I mean PUSH! It takes a bit of effort, but make sure you get it all the way in. (TWSS)  
![PXL_20231220_142429565](https://github.com/IRTrail/Voron-Stuff/assets/53546870/0e34f2db-9504-40ac-ba4d-af43514da0a3)  

Here's the tube seated in the extruder body:  
![PXL_20231220_142527996](https://github.com/IRTrail/Voron-Stuff/assets/53546870/49bd3322-76a1-4ed9-ab66-ba7b9bd680b4)  

##### Step 6:  
Trim the tube flush with the drilled out heat set:  

###### Notes:
I am not entirely sure how much the heat set helps. I *think* it was intended to create a nice hard surface to shear against the blade. However, it seems to work well with the PTFE tube in there. If I get to the point that I print another extruder body, I'll try one without the heatset and a bore sized for the PTFE tube instead.
