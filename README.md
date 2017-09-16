# Glowdeck_Wifi
Tools for working with the Wifi module on the Glowdeck board


NOTES

•    This folder should contain the wifi firmware and web client bin files: Firmware_V3.2.bin and Website_V3.7.bin

•    Depending on when you downloaded this firmware update package, the bin files in this folder might not be the most recent builds. To ensure you have the newest builds, you can always replace the files currently residing in this folder with the bin files hosted at: http://j.mp/usrfirmware and http://j.mp/usrwebsite (respectively).  Please note that the files you download from these URLs may have slightly different names, but should still indicate their version numbers (e.g. firm_v3.2.bin).

INSTRUCTIONS

1.    Unplug the Glowdeck PCB. Then, while pressing and holding down the front button, connect power to the DC barrel jack in the back of your PCB (using the provided 12V power adapter). 
2.    The LEDs will all turn on (in either red or blue), and you can let go of the front button.

3.    Search for Wifi networks on the computer containing the bin files. When you see either “GlowdeckXXXXX” (where XXXXX are 5 letters/numbers) or “USR-WIFI232-T” appear in the list of found networks, click to connect to that network.

4.    Once connected, open a web browser and go to the URL: 10.10.100.254/iweb.html (if it prompts you for a username/password, either admin/admin or glowdeck/glowdeck should work).

5.    First click the browse for firmware button (the top option) and select the Firmware_V3.2.bin file. Then click upload and wait a few seconds. If the upload succeeds, you will be taken to a page that reads “Update successful!” If not, go back to the original URL and try again. 
6.    Power cycle your Glowdeck board and restart again in DFU mode (per step 1). Now repeat steps 2-5, but this time upload the Website_V3.7.bin file using the custom website field (the bottom option). Note that this will take about 10-20 seconds, but will land on an error page even if it succeeds. You can verify it worked by checking the URL of the page that it failed to load, and it should be: 10.10.100.254/data_success.html


*The files in this package are not intended for public distribution. The firmware update procedure described herein should be followed exactly as-written, and only by persons with some degree of familiarity with embedded development.


DISCLAIMER:
By proceeding to update or modify the firmware on the Glowdeck PCB (and/or on one of its constituent components/modules), you assume full responsibility for any resultant outcome. You acknowledge that one such outcome of a firmware modification/update can be the rendering of one or more modules of the Glowdeck PCB dysfunctional (whether temporary or permanent). Contact support@streams.io before proceeding and wait for a response if you have any questions.
