# Zonestar3DNotesAndTricks

Here I will publish what can solve or improve with my 3D printer Zonestar Z8PM4-MK2 

### 05-24-24
First challenge was run Ultimate Cura  in ubuntu 22.04 Following official  [tutorial](https://www.youtube.com/watch?v=h2GynyUo7wQ) 
after download [zonestar resources](https://github.com/ZONESTAR3D/Slicing-Guide/tree/master/cura) and copy that in
`~/.local/share/cura/5.7`, however, slice can't be doing.   

The solution was update the definitions with latest version from Cura and merge it with Zonestar definitions. 
Cura resources location:
 - [fdmextruder-def](https://github.com/Ultimaker/Cura/blob/main/resources/definitions/fdmextruder.def.json)
 - [fdmprinter-def](https://github.com/Ultimaker/Cura/blob/main/resources/definitions/fdmprinter.def.json)
 
 In Resources are alocated the updated files that worked for me. 
 

to run cura first time in my laptop bench i need to install  libfuse2
sudo apt install libfuse2

### 06-05-2024
I configured cura with my arbitrate parameters to print. I test the setups printing a Rapberry pi 4 case. 
I get the models from [thingiverse](https://www.thingiverse.com/thing:3948992) and the parameter was:
- **Quality**:
    - Layer Height: **0.3 mm**
    - Initial layer height: **0.35mm**
    - Line width: **0.4mm**
- **Walls**    
    - Wall thickness: **0.8mm**
    - Wall line count: **3**
- **Infill**
    - Infill density: **20%**
    - Infil pattern: **Tri-hexagon**
- **Material**
    - Printing temperature: **235**  
    - Printing temperature: initial layer: **240**
    - Bed temperature: **70**
    - Bed temberature initial layer: **75**
- **Speed**    
    - Print speed: **37.0 mm/s**
    - Travel speed: **120**
- **Travel**
    - Retraction distance: **12.0mm**
    - Retraction speed: **30.0mm**
- **Cooling**
    - Fan speed: **50%**

The material that I used is PetG of [KingRoon](https://es.aliexpress.com/item/1005004832752591.html?spm=a2g0o.order_list.order_list_main.54.3f15194dMfs7l8&gatewayAdapt=glo2esp) brand with next parameters:
- Density: **1.24g/cm3**
- Diameter: **1.75mm**
- Default printing temperature: **235º C**
- Retraction distance: **1mm**
- Retraction Speed: **20mm**
- Fan Speed: **50%**



