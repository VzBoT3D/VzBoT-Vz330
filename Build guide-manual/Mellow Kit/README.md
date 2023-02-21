# This page is a WIP (Work in Progress)

Additional information for Kit owners/builders. In this section you can find more information for the build process and evolution of the project.
This is still a beta release, and we will try our best to help you through this build.

# What do I need to print?:

This section will help to determine what you need to print in advance for the build. It will be devided by section and STLs can be found in the [Assemblies BOM and STL](/Assemblies%20BOM%20and%20STL)

## [Alignment tools](/Assemblies%20BOM%20and%20STL/Alignment%20Tools): 
- [Z alignment tool for 10mm Rods](/Assemblies%20BOM%20and%20STL/Alignment%20Tools/Z%20Alignment%20tool%2010mm%20rod.stl) x2
- You do not need to print the MGN rail alignment tool(s) as the gantry is pre-assembled.

## [Frame](/Assemblies%20BOM%20and%20STL/Frame)
<img width="607" alt="image" src="https://user-images.githubusercontent.com/37383368/210115146-2aabb50a-7a39-4201-ad02-35352c372164.png">
- All the STL found in the frame section, except the rear top brace for motor tensioner. (These braces are for people running with no enclosure)
- Some users reported that the 20mm M4 bolts and tnuts were missing from the kit for the 4 frame feet. You might have to source them

## [Gantry](/Assemblies%20BOM%20and%20STL/Gantry):
<img width="1093" alt="image" src="https://user-images.githubusercontent.com/37383368/210687358-556ff2ba-ccea-4c6a-bc5b-d21a3601e608.png">
<img width="377" alt="image" src="https://user-images.githubusercontent.com/37383368/210686948-ba47410a-75ec-418b-a01f-66142b5d66fa.png">

## Gantry comes pre-assembled with printed parts in PLA that are for transportation only. It should not be used on the printer. You can easily replace the parts without disassembling the whole thing.

### [Y gantry](/Assemblies%20BOM%20and%20STL/Gantry/Y%20gantry/Aluminum%20Y%20Gantry)
- [Y gantry tube spacers](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/Gantry/Y%20gantry/Aluminum%20Y%20Gantry/STLs/spacer_alu_Y_gantry_0.5mm.stl) x4 (Make sure to read instructions in the link above)
- [Y gantry back spacers](/Assemblies%20BOM%20and%20STL/Gantry/Y%20gantry/Aluminum%20Y%20Gantry/STLs/gantry%20back%20spacer.stl) x2
- [X limit switch stopper](/Assemblies%20BOM%20and%20STL/Gantry/Y%20gantry/Aluminum%20Y%20Gantry/STLs/XendStop.stl)
### [Rear motor mounts](/Assemblies%20BOM%20and%20STL/Gantry/Motor%20Mounts/Aluminum)
- [spacer frame side](/Assemblies%20BOM%20and%20STL/Gantry/Motor%20Mounts/Aluminum/Left%20Motor%20Mount/STLs/Spacer%20frame%20side.stl) x2
- [spacer inner side](/Assemblies%20BOM%20and%20STL/Gantry/Motor%20Mounts/Aluminum/Left%20Motor%20Mount/STLs/Spacer%20inner%20side.stl) x2
- [Tension adjustement knob](/Assemblies%20BOM%20and%20STL/Gantry/Motor%20Mounts/Aluminum/Left%20Motor%20Mount/STLs/knob.stl) x2
- [knob cap](/Assemblies%20BOM%20and%20STL/Gantry/Motor%20Mounts/Aluminum/Left%20Motor%20Mount/STLs/knob-cap.stl) x2
### [Front motor mounts](/Assemblies%20BOM%20and%20STL/Gantry/Front%20Idler-motor%20mounts%20AWD/Alu%20version)
- [Spacers](/Assemblies%20BOM%20and%20STL/Gantry/Front%20Idler-motor%20mounts%20AWD/Alu%20version/20mmSpacer.stl) x2

### Y limit switch mount is CNC. No need to print it


NOTE: The motor/idler mounts may have been assembled the wrong position for the idlers. Refer to the CAD model [here](https://a360.co/3Q0ueRY) to make sure they are properly installed. Also something that we didn’t think about for the pre-assembled gantry, is that you will need to unbolt the front motor/idler full assembly in order to access the M5 frame bolt on both sides (refer to screen shot here). No need to disassemble the whole assembly, just remove the bolts that holds both aluminum plates to the frame so you can remove the whole assembly as one. ![image](https://user-images.githubusercontent.com/37383368/210116584-4fd1e248-d878-4ef8-8ca3-ec01c82c4c76.png)

- A good practice here on the 4 motors would be to make sure that motor gears are bolted to motor shaft on the round side of the shaft and NOT using the D cut out (the flat portion of the shaft) before you install the belts. This will help your later to sync all motors together. If the gears are installed on the D cut, then synching is impossible to achieve. Gears need to be able to adjust their position on the shaft. The build manual will explain you how to sync the motors later [here](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Build%20guide-manual/VZ330%20AWD%20Manual%20Aluminum.pdf)


## [Printhead](https://github.com/VzBoT3D/Vz-Printhead/)
<img width="450" alt="image" src="https://user-images.githubusercontent.com/37383368/210114952-d4b98c4c-af4c-41a7-8c46-ad2d894253c3.png">
### NOTE: 4xM3 4mm should have been included in the kit to mount the printhead to the MGN9. Some people reported those 4 were missing. If that is your case, please use the M3x4 button head. It should work. If you prefer you could grind down the included M3x6mm bolt about 1mm so it's 5mm. Insert a nut on the bolt before doing so, that way when you are done grinding (or cutting), the threads will be repaired when the nut is removed. 
<img width="317" alt="image" src="https://user-images.githubusercontent.com/37383368/210915792-5fe2450f-fd8d-4cbe-bf2e-e2d220632499.png">

- A 22mm PTFE tube is needed between the Goliath and Vz-HextrudORT. A capricorn style tube (1.9mm ID) is also recommended.

- [X end stop switch mount](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/X-endstop-mount.stl)
- [cable holder ](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/cable_holder.stl)
- [fan duct lower Goliath](https://github.com/VzBoT3D/Vz-Printhead-CNC/blob/main/STLs/fan%20duct%20lower%20Goliath%20long.stl)
- [fan duct lower Goliath spacers](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/fan%20duct%20lower%20Goliath%20spacers.stl)
- [fan duct upper](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/CPAP%20turbo%20cooling%20system/STLs/upper%20duct.stl)
- [upper duct mount](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/CPAP%20turbo%20cooling%20system/STLs/upper%20duct%20mount.stl)
- [upper duct cpap c clamp](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/CPAP%20turbo%20cooling%20system/STLs/c-clamp.stl)
- [Goliath 2510 fan duct](https://github.com/VzBoT3D/Goliath/blob/main/STL/Air%20Cool%20Fan%20duct/Fan%20duct%202510-With%20flange%20for%20Vz-Printhead%20CNC.stl)
<img width="300" alt="image" src="https://user-images.githubusercontent.com/37383368/214460290-3fa1b67c-b6f5-406e-973e-913280dc1212.png">


## [Z complete system (pdf manual here)](/Assemblies%20BOM%20and%20STL/Z%20complete%20system%20-%20Aluminum)
<img width="709" alt="image" src="https://user-images.githubusercontent.com/37383368/210116113-fcefb1c3-d0aa-4042-86ad-bc0f0d15b7de.png">

(Cable chain is missing/not included in the beta kits. Some people prefer a umbilical chord with wire sleeve/loom. If you wish to buy a chain, get a 10x10 chain with the end joints here or similar https://s.click.aliexpress.com/e/_DDGBfvz. One end bolts to frame with M3 tnuts and bolts and the other end bolts to the printed mount on the bed support plate)

(some customers reported missing bed silicon spacers in their kit. Kit comes with clear translucent spacers, but i recommend black silicon spacers. Check in the bom for link. We will try to fix this on the next kits. If you buy the black spacers, you can use a big metal washer 20mm between spacer and heat bed)

- [Bed level adjustment knobs](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/Z%20complete%20system%20-%20Aluminum/STLs/Bed%20level%20adjustment%20knobs%20.stl)
- (For chain mount, if your bed support plate don’t have the 2 M3 holes/thread in the back please use chain mount option2)
- [Z-chain mount](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/Z%20complete%20system%20-%20Aluminum/STLs/Z-chain%20mount.stl)
- [Z-chain mount option2](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/Z%20complete%20system%20-%20Aluminum/STLs/Z-chain%20mount%20option2.stl)
- [Z-chain mount option2-spacer](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/Z%20complete%20system%20-%20Aluminum/STLs/Z-chain%20mount%20option2-spacer.stl)
- [Z stop switch mount](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/Z%20complete%20system%20-%20Aluminum/STLs/printed%20z%20switch%20adapter.stl) There is a STL for that, but the kit comes with a CNC switch mount. 

## [RSCS](/Assemblies%20BOM%20and%20STL/RSCS)
<img width="574" alt="image" src="https://user-images.githubusercontent.com/37383368/210115893-5dd6f5ff-7716-4ad3-bcb9-101bca8e2e98.png">
(Print 2 times)

- [Lower duct](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/RSCS/STLs/Lowerduct.stl)
- [middle high duct](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/RSCS/STLs/MiddleHigh-duct.stl)
- [middle low duct](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/RSCS/STLs/MiddleLow-duct.stl)
- [top duct](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/RSCS/STLs/Top-duct.stl)

## [Enclosure](https://github.com/VzBoT3D/VzBoT-Vz330/tree/master/Assemblies%20BOM%20and%20STL/enclosure)
![image](https://user-images.githubusercontent.com/37383368/210599061-ed3ba344-b45c-4c4e-884d-f9e488dcd232.png)

- You need everything in link above

## [Electronics](/Assemblies%20BOM%20and%20STL/electronics)

## [Back Electronic bay](/Assemblies%20BOM%20and%20STL/electronics/Back%20Electronic%20bay):
can be customized to your liking. We suggest one design that you can use on github if you wish
<img width="775" alt="image" src="https://user-images.githubusercontent.com/37383368/210691792-242bcd64-5d62-46c1-8cf6-ed17f6778346.png">
- [CPAP controller board mounting plate](/Assemblies%20BOM%20and%20STL/electronics/Back%20Electronic%20bay/CPAP%20controller%20board%20mounting%20plate.stl) M2.5 screws to secure the board to printed mount, and use double sided tape to mount to the back plate
- [CPAP fan mount](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/CPAP%20turbo%20cooling%20system/STLs/CPAP%20fan%20mount.stl)
- [CPAP fan outlet](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/CPAP%20turbo%20cooling%20system/STLs/CPAP%20fan%20outlet%20adapter.stl)
- [Lower Grill right with powerswitch](/Assemblies%20BOM%20and%20STL/electronics/Back%20Electronic%20bay/Lower%20Grill%20right%20with%20powerswitch.stl) (can be mirrored in slicer if you wish to have the POWER line and switch on the left side)
- [Lower Grill left](/Assemblies%20BOM%20and%20STL/electronics/Back%20Electronic%20bay/Lower%20Grill%20left.stl) (can be mirrored in slicer)
- [Super8 +5160 mount](/Assemblies%20BOM%20and%20STL/electronics/Back%20Electronic%20bay/Fly%20Super8/FlySuper8%2B4x5160pro%20mount.stl)
- [Super8 din mount](/Assemblies%20BOM%20and%20STL/electronics/Back%20Electronic%20bay/Fly%20Super8/FlySuper8%20din%20mountX2.stl) x2
- [5160 fan cover](/Assemblies%20BOM%20and%20STL/electronics/Back%20Electronic%20bay/Fly%20Super8/FlySuper8%20fan%20cover.stl)
- [knobs](/Assemblies%20BOM%20and%20STL/electronics/Back%20Electronic%20bay/knobs.stl) x4
- [Vz330 logo plate](/Assemblies%20BOM%20and%20STL/electronics/Back%20Electronic%20bay/Vz330%20logo%20plate.stl)
- Raspberry pi DIN mount. Your personal preference. Some models found [here](https://www.printables.com/search/all?q=raspberry%20pi%20din)

## [Front screen mount](/Assemblies%20BOM%20and%20STL/electronics/Screen%20Mount/New%20Version)
<img width="742" alt="image" src="https://user-images.githubusercontent.com/37383368/210694491-ad33eb76-7252-42f3-8e87-412ff7cd0f20.png">

- [Screen mount back](/Assemblies%20BOM%20and%20STL/electronics/Screen%20Mount/screen%20mount%20back.stl)
- [Screen mount frame](/Assemblies%20BOM%20and%20STL/electronics/Screen%20Mount/screen%20mount%20frame.stl)
- [Screen front cover](/Assemblies%20BOM%20and%20STL/electronics/Screen%20Mount/New%20Version/screen%20cover.stl)
- [Screen back](/Assemblies%20BOM%20and%20STL/electronics/Screen%20Mount/New%20Version/screen%20back.stl)

## Optional:

- [Front LED](/Assemblies%20BOM%20and%20STL/electronics/Front%20LED%20for%20AWD)

...... work in progress..
