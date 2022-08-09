Assembling the print head is straight forward.

# Step 1 : Mounting the Fan and Cable holder.
![image](https://user-images.githubusercontent.com/37383368/144164913-77f6e690-bd68-4acc-98df-f23f697ef434.png)
## BOM needed:
- 4xM3 6mm Ultra low profile bolts
- cable holder (printed)

# Step 2 : Assembling the carriage
- Install the top plate on the X MGN9 slider
- Install the back, front, and bottom plates
![image](https://user-images.githubusercontent.com/37383368/144165073-5143faec-5863-466d-8608-cd1a1402f1c1.png)

## BOM needed:
- 12xM3 6mm Ultra low profile bolts (For all 8 corners and MGN9 bloc)


# Step 3: Mounting the the X stop switch (Optional: if you don't use sensorless homing)
![image](https://user-images.githubusercontent.com/37383368/144165516-71b350dc-e5e7-4ad3-9994-2b5eeb7d3ebf.png)
### Rat Rig Vcore3 users: You will need to add this X stopper to your Left Xy joiner. STL found [here](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/PrintHeads/Vz-Print%20Head%20Alu-CF/STLs/Vcore3%20specific/Vcore3_X_stopper.stl) 
Please note that you will need a 15mm M5 bolt instead of a 12mm
![image](https://user-images.githubusercontent.com/37383368/166172614-6126112e-fe90-472b-8d7b-c416a6c2a4d1.png)

Also, you can re-use the Vcore original X switch with this [mount](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/PrintHeads/Vz-Print%20Head%20Alu-CF/STLs/Vcore3%20specific/X-endstop-mount.stl)

## BOM needed:
- 2 x M3 6mm Ultra low profile bolts
- 2 x M2 screws (not included in the kit)
- Microswitch https://s.click.aliexpress.com/e/_AL9anj
- Switch mount (Printed)

# Step 4: Install the rear adjustable fan mount
![image](https://user-images.githubusercontent.com/37383368/144165782-2720e21d-af35-439d-a1e4-e043f39f8716.png)
## BOM needed:
- 2 x M3 8mm Ultra low profile bolts
- 2 x M3 Nuts

# Step 5: Install the belts.
- make sure motor mounts are a lowest tension possible first.
- Start by the front. Insert the end of the belt through the side slot and loop the belt on itself. Insert a piece of filament (6mm) in the loop and then slowly pull the belt back in the slot until secures in place.
- For the back, simply loop the belt arround the pillar, and give it a pre-tention on the belt, then attach it with a zip tie, or a printed belt clip (Found in the [STL](https://github.com/VzBot3D/VzBot/tree/master/Assemblies%20BOM%20and%20STL/PrintHeads/Vz-Print%20Head%20Alu-CF/STLs) folder) . [belt clip](https://github.com/VzBot3D/VzBot/blob/master/Assemblies%20BOM%20and%20STL/PrintHeads/Vz-Print%20Head%20Alu-CF/STLs/Belt_clip.stl)
- [![belts-installation](https://user-images.githubusercontent.com/37383368/146992012-26b7d4e9-f979-4afb-9dfe-6e3e31b0ecac.jpg))](https://youtu.be/Ibi27Toh-pg)
- (For Vz235, you can use 2 techniques described here in this [video](https://www.youtube.com/watch?v=lP59PClF_PU&t=3334s). For the optional 2 piece clips, here they [are](https://github.com/VzBoT3D/VzBoT-Vz235/tree/main/Assemblies%20%26%20STL/Gantry/Misc))




# Step 5.1
Take a rum shot. This step is definately needed after the belts job. It takes a bit of patience to route the belts in the front idlers, with a small screw driver, its very doable

# Step 6: Install the fan duct
![image](https://user-images.githubusercontent.com/37383368/144167630-18dacba9-8475-4689-8376-9929f1c42db1.png)
## BOM needed:
- 2 x M3 10mm bolts
- 2 x M3 Nuts
- Upper fan duct (printed)
- Lower fan fuct (printed)

# Step 7: Install your favorite extruder/hotend combo.
Refer to the sections above (or links down below)for instructions and BOM
- [BOWDEN](https://github.com/VzBot3D/VzBot/tree/master/Assemblies%20BOM%20and%20STL/PrintHeads/Vz-Print%20Head%20Alu-CF/MGN9%20version/BOWDEN)
- [Direct Drive](https://github.com/VzBot3D/VzBot/tree/master/Assemblies%20BOM%20and%20STL/PrintHeads/Vz-Print%20Head%20Alu-CF/MGN9%20version/Direct%20Drive)

# Step 7.1
Take a second well deserved rum shot. Please note that beer can be used in this step.

# Step 8 : Adjust the fan height
Loosen the 2 M3 8mm bolts, and ajust height according to your Hotend
![image](https://user-images.githubusercontent.com/37383368/144168574-4e82006d-b79b-4e37-b99f-34f7c00d5af3.png)

# Step 9 : Install the 5015 fan with optional BL Touch mount (More probe type will be supported later)
![image](https://user-images.githubusercontent.com/37383368/144168824-7156b8d9-2fe7-4098-915b-31f145dcd3d1.png)
![image](https://user-images.githubusercontent.com/37383368/144168882-fc4419c9-49b1-4dae-bfeb-97a5b0f7b51a.png)
![image](https://user-images.githubusercontent.com/37383368/157687995-3fd05f2c-27e8-4a83-980b-1fac1bc3e35d.png)

# Option : Tri horn fan duct with brace (useful when running a z probe sensor)
If you find that your fan duct is not stiff enough and move after a while, this mod of the fan [duct](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/PrintHeads/Vz-Print%20Head%20Alu-CF/STLs/fan%20duct%20lower%20body-trihorn%20with%20brace.stl) is for you. Scale the [spacers](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/PrintHeads/Vz-Print%20Head%20Alu-CF/STLs/fan%20duct%20lower%20body-brace%20Z%20scalable%20spacers.stl) according the the height needed.
![image](https://user-images.githubusercontent.com/37383368/176760266-9fbbe036-2285-433d-9bbc-f1edfe9d210f.png)


# Optional : Cable mount brace
If you do not need to bring the fan all the way down, you can print and install this little [BRACE](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/PrintHeads/Vz-Print%20Head%20Alu-CF/STLs/cable_mount_brace_brace.stl) that will help secure the cable mount in place
![image](https://user-images.githubusercontent.com/37383368/173377071-cb560330-bb4c-449d-8ee5-06435b12b3f9.png)

# Optional : Klickyand Quickdraw probe: 
Fan duck with probe: [Here](https://grabcad.com/library/contribution-to-the-various-vzbot-fanduct-systems-in-combination-with-the-klicky-probedi-jlas1-and-quickdraw-systems-of-annex-1?fbclid=IwAR16A_0Nun4rFj4dr5-l7O6l62gWpChDlT06tSl2N-mH0tbDB2Qwea59Pus)
Docking system: [Here](https://grabcad.com/library/contribution-to-the-retractable_probe_dock-for-klicky-probe-and-quickdraw-probe-system-for-voron-of-tronfu-adapted-to-vzbotrobe-per-voron-di-tronfu-riadattato-alla-vzbot-1?fbclid=IwAR31FLcYtxWH4eCrtFb1iTl6fMMfGeksUfxyhcuGlu9bqLtTKSHHada0CzA)
![image](https://user-images.githubusercontent.com/37383368/176207407-0eb39f79-caba-44fd-b1ec-83fbe20a3baf.png)
![image](https://user-images.githubusercontent.com/37383368/176208539-eac2eba9-f4ca-4651-94b0-fdf6f2e59ec2.png)



## BOM needed:
(No probe):
- 1 x M3 20mm bolt - (For right side of the fan when you face printer - When NOT using probe)
- 1 x M3 25mm bolt - (for left side  Please note the left side bolt orientation is different to clear the belt)
- 1 M3 8mm (upper fan duct brace)
- 3 x M3 Nuts
(With probe):
- 2 x M3 25mm bolt - (Please note the left side bolt orientation is different to clear the belt)
- 1 x M3 8mm (upper fan duct brace)
- 2 x M3 6mm (Bltouch mount


