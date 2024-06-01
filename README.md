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
