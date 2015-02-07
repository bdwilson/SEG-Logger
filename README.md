SmartThings SmartApp Energy Logger for SmartEnergyGroup (SEG)
=======
<br>
SmartThings SmartApp to send energy meter data (kWh and watts) to
www.smartenergygroups.com.  Testing with HEMv1 but will likely work with any
device that supports EnergyMeter capabilities with SmartThings.

<b>NOTE: I've received inconsistent results with energy measurement (kWh) using my
HEMv1 and SEG. I have attempted to seek help from the SEG maintainer, but
nothing has been resolved. If you want to help me resolve, you can start here:
https://smartenergygroups.com/forums/10-The-Open-Grid/topics/352-Posting-kWH-to-the-API
If you're looking for reliable cost calculations, then PlotWatt is a better
option for now. </b>

Requirements
------------
- SmartThings HUB
- Device that supports the "EnergyMeter" capability (tested with HEMv1)
- [SEG Account](https://smartenergygroups.com/) - FREE

Installation
--------------------
1. Create a SEG account and create a new site.
2. Add a device to the site and select "Energy Meter". The name can be
anything, but the <b>node name must be the Display Name of your Energy Device
from [SmartThings](https://graph.api.smartthings.com/device/list) AND you must
replace all spaces with underscores and remove parenthesis!</b> For instance, if my device is
called "Panel 1 (Generator)" my node name in SEG would be Panel_1_Generator.
This should create you a Power and Energy section.
3. Edit both the Power and Energy sections, click Edit and change their stream
names to "power" and "energy" respectively. Check the kilo option if you want
your data displayed in kWh.
4. Repeat steps 2-3 for each EnergyMeter device you want to monitor.
5. Now, add a [SmartApp](https://graph.api.smartthings.com/ide/apps) and do from Source Code.  
6. Save and publish the app. 
7. Go to your phone, +, add Smart App and add the
[site_token](https://smartenergygroups.com/my_things/show_keys) from SEG to
your app and select the energy meters, or you can add your App to the devices
from the IDE on the SmartThings website.  

Options
-----------------
If for some reason you want to run this as a scheduled job instead of when
subscribed activity from your meter triggers this, review the Initialization
subroutine to adjust how it is called.

Bugs/Contact Info
-----------------
Bug me on Twitter at [@brianwilson](http://twitter.com/brianwilson) or email me [here](http://cronological.com/comment.php?ref=bubba).


