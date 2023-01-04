# This page is a WIP (Work in Progress)

Additional information for Kit owners/builders. In this section you can find more information for the build process and evolution of the project.
This is still a beta release, and we will try our best to help you through this build.

# What do I need to print?:

This section will help to determine what you need to print in advance for the build. It will be devided by section and STLs can be found in the [Assemblies BOM and STL](/Assemblies%20BOM%20and%20STL)

## [Alignment tools](/Assemblies%20BOM%20and%20STL/Alignement%20Tools): 
- [Z aligment tool for 10mm Rods](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/Alignement%20Tools/Z%20Alligment%20tool%2010mm%20rod.stl)
- You do not need to print the MGN rail aligment tool(s) as the gantry is pre-assembled.

## [Frame](/Assemblies%20BOM%20and%20STL/Frame)
<img width="607" alt="image" src="https://user-images.githubusercontent.com/37383368/210115146-2aabb50a-7a39-4201-ad02-35352c372164.png">
- All the STL found in the frame section, except the rear top brace for motor tensioner. (These braces are for people running with no enclosure)
- Some users reported that the 20mm M4 bolts and tnuts were missing from the kit for the 4 frame feet. You might have to source them

## [Gantry](/Assemblies%20BOM%20and%20STL/Gantry):
<img width="992" alt="image" src="https://user-images.githubusercontent.com/37383368/210115639-6b2158bb-fa36-4a1c-9ae3-acfcb1e5f99b.png">
<img width="550" alt="image" src="https://user-images.githubusercontent.com/37383368/210115736-cbf3270c-41dd-4773-b718-5142a84d999d.png">

- [Y gantry tube spacers](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/Gantry/Y%20gantry/Aluminum%20Y%20Gantry/STLs/spacer_alu_Y_gantry_0.5mm.stl) x4

- Gantry comes pre-assembled with most printed parts already there. You will only need the X tube spacers. Mesure you CF tube in height. If your tube is 20mm tall, then you will need to print 4 spacers (2 on each side) of 0.5mm. The Y gantry has an opening of 21mm, so you will need to compensate for 1mm if your tube is 20mm. So 0.5mm spacers between Y gantry and tube. (One top and one bottom to keep it centered). If your tube is 20.5mm, then you have a 0.5mm to compensate, so print spacers with 0.25mm height (scale them in Z in your your slicer to the desired height).

- The front motor/idler mounts on X1 side maybe have been assembled the wrong way for the idlers. Refer to the CAD model or the screenshot below. Also something that we didnt think about for the pre-assembled gantry, is that you will need to unbolt the front motor/idler full assembly in order to access the M5 frame bolt on both sides (refer to second screen shot here). No need to dissassemble the whole assembly, just remove the bolts that holds both aluminum plates to the frame so you can remove the whole assembly as one. 

- A good practice here on the 4 motors would be to make sure that motor gears are bolted to motor shaft on the round side of the shaft and NOT using the D cut out (the flat portion of the shaft) before you install the belts. This will help your later to sync all motors together. If the gears are installed on the D cut, then synching is impossible to achieve. Gears need to be ablet to adjust their position on the shaft. The build manual will explain you how to sync the motors later [here](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Build%20guide-manual/VZ330%20AWD%20Manual%20Aluminum.pdf)
<img width="850" alt="image" src="https://user-images.githubusercontent.com/37383368/210116456-26c591d4-d10b-4140-baf6-b5b4c1545568.png">

![image](https://user-images.githubusercontent.com/37383368/210116584-4fd1e248-d878-4ef8-8ca3-ec01c82c4c76.png)



## [Printhead](https://github.com/VzBoT3D/Vz-Printhead/)
<img width="450" alt="image" src="https://user-images.githubusercontent.com/37383368/210114952-d4b98c4c-af4c-41a7-8c46-ad2d894253c3.png">

- [X endstop switch mount](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/X-endstop-mount.stl)
- [cable holder ](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/cable_holder.stl)
- [fan duct lower Goliath](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/fan%20duct%20lower%20Goliath.stl)
- [fan duct lower Goliath spacers](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/fan%20duct%20lower%20Goliath%20spacers.stl)
- [fan duct upper](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/CPAP%20turbo%20cooling%20system/STLs/upper%20duct.stl)
- [upper duct mount](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/CPAP%20turbo%20cooling%20system/STLs/upper%20duct%20mount.stl)
- [upper duct cpap c clamp](https://github.com/VzBoT3D/Vz-Printhead/blob/main/STLs/CPAP%20turbo%20cooling%20system/STLs/c-clamp.stl)

## [Z complete system (pdf manual here)](/Assemblies%20BOM%20and%20STL/Z%20complete%20system%20-%20Aluminum)
<img width="709" alt="image" src="https://user-images.githubusercontent.com/37383368/210116113-fcefb1c3-d0aa-4042-86ad-bc0f0d15b7de.png">

(Cable chain is missing/not included in the beta kits. Some people prefer a ombilical chord with wire sleeve/loom. If you wish to buy a chain, get a 10x10 chain with the end joints here or similar https://s.click.aliexpress.com/e/_DDGBfvz. One end bolts to frame with M3 tnuts and bolts and the other end bolts to the printed mount on the bed support plate)

(some cusotmers reported missing bed silicon spacers in their kit. Kit comes with clear translucent spacers, but i recommend black silicon spacers. Check in the bom for link. We will try to fix this on the next kits. If you buy the black spacers, you can use a big metal washer 20mm between spacer and heatbed)

- [Bed level adjustment knobs](https://github.com/VzBoT3D/VzBoT-Vz330/blob/master/Assemblies%20BOM%20and%20STL/Z%20complete%20system%20-%20Aluminum/STLs/Bed%20level%20adjustment%20knobs%20.stl)
- (For chain mount, if your bed support plate dont have the 2 M3 holes/thread in the back please use chain mount option2)
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


...... work in progress.. 
