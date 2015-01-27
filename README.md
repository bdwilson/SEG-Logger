SmartThings SmartApp Energy Logger for SmartEnergyGroup (SEG)
=======
<br>
Shell script-based MythTV User Job to transcode recordings to mp4, retrieve
metatata, and update XBMC. This does not alter the MythTV content at all.
Requirements
------------
- SmartThings HUB
- Device that supports the "EnergyMeter" capability (tested with HEMv1)
- [SEG Account](https://smartenergygroups.com/) - FREE

Installation
--------------------
1) Create a SEG account and create a new site.
2) Add a device to the site and select "Energy Meter". The name can be
anything, but the <b>node name must be the Display Name of your Energy Device
from [SmartThings](https://graph.api.smartthings.com/device/list) AND you must
replace all spaces with underscores and remove parenthesis!</b> For instance, if my device is
called "Panel 1 (Generator)" my node name in SEG would be Panel_1_Generator.
This should create you a Power and Energy section.
3) Edit both the Power and Energy sections, click Edit and change their stream
names to "power" and "energy" respectively. <b>Make sure you check kilo option
for energy.</b>
4) Replease steps 2-3 for each EnergyMeter device you want to monitor.
5) Now, add a [SmartApp](https://graph.api.smartthings.com/ide/apps) and do
from Source Code.  
6) Save and publish the app. 
7) Go to your phone, +, add Smart App and add the
[site_token](https://smartenergygroups.com/my_things/show_keys) from SEG to
your app and select the energy meters.  

Bugs/Contact Info
-----------------
Bug me on Twitter at [@brianwilson](http://twitter.com/brianwilson) or email me [here](http://cronological.com/comment.php?ref=bubba).


