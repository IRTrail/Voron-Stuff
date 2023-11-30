# Trouble getting the CANBUS UUID?
## _Here's the nuclear option:_
If you're flashing a component that has previously had klipper running on it, you'll need to ensure no traces of the former Klipper install exist in the flash memory, or `~/katapult/scripts/flash_can.py -i can0 -q` will not show the UUID.
For instance, I tried to flash my Mellow Super 8 from using USB communication to CANBUS, and was unable because the UUID was elusive. I tried evry which way I could and finally recieved help from Esoterical on the Voron discord.
The solution is:
`dfu-util -R -a 0 -s 0x08000000:force:mass-erase:leave -D ~/katapult/out/katapult.bin -d <serial id>`
This essentially nukes the old Klipper install, ensuring the only thing on the board is the Katapult boodloader install. After running this command, the UUID query worked flawlessly and I was able to proceed with the rest of the Klipper CANBUS install.

I hope this helps someone out there.
