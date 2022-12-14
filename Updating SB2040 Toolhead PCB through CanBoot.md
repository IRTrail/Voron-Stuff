# Updating your SB2040 via CanBoot
  When I saw the dreaded "update" symbol in Mainsail next to Klipper, I knew it was time to hit up KIAUH. The problem is, I had just switched over to CAN Bus and that meant I had another MCU to update.
  Scouring the interwebs for clues as to how to accomplish this feat revealed that there really isn't a great write up on it.
  It's probably tribal knowledge throughout the Klipper community, but I just wasn't in the tribe.
  So, thanks to a bit of explaination from DonnerPlays on the 3DMellow section of the Voron Discord, the answer was revealed.
  Hopefully this helps someone in the future.
  
## The process
  The main process is pretty much the same as flashing Klipper after flashing CanBoot:
  1. SSH into your Pi
  2. ```cd ~/klipper
    make clean
    make menuconfig
    ```  
    You should have the following options for the SB2040 and CanBoot:
    ![Alt Image text](https://user-images.githubusercontent.com/53546870/207622631-bedbdb38-ff9e-4ac0-97b7-44708631663f.png, "menuconfig")
