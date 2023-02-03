# PNR-Lab
# Advance Physical Design using OpenLANE/Sky130

 ![image](https://user-images.githubusercontent.com/123365348/216224286-7692e544-e931-47fb-9e35-94b2c5bd8641.png)

  # Prepared Design
  ![image](https://user-images.githubusercontent.com/123365348/216225497-4b7cf8d5-3618-4eba-9c00-0e3136b9b6ba.png)

![image](https://user-images.githubusercontent.com/123365348/216226243-767c9633-1481-4952-b8b9-74433ee34800.png)

![image](https://user-images.githubusercontent.com/123365348/216226801-cc1cc3c7-aa91-4df6-9b1a-2cbbbb7c3ef6.png)
![image](https://user-images.githubusercontent.com/123365348/216226996-de58ec06-9723-49dc-8c05-b9d55560f65f.png)

cd tmp
less merged.lef

![image](https://user-images.githubusercontent.com/123365348/216228904-243c286c-1524-4b52-8031-bccb4c48131b.png)

cd ../
clear
cd results
![image](https://user-images.githubusercontent.com/123365348/216229126-3e6a90c5-774f-4d99-8e74-3d5897fccb12.png)

cd ../
cd reprots
ls -ltr
![image](https://user-images.githubusercontent.com/123365348/216229418-3fa46a2b-1521-445b-8991-673cf756f102.png)

cd ../
less config.tcl
![image](https://user-images.githubusercontent.com/123365348/216229603-3c118c96-fbd4-42f2-9570-357dfde7b0f4.png)
less cmds.log
![image](https://user-images.githubusercontent.com/123365348/216229689-461d8c35-ef4c-4409-81af-0600eb69a57f.png)

%run_synthesis
![image](https://user-images.githubusercontent.com/123365348/216229981-f2762adb-9621-4e83-b9c3-6a788a6a67c0.png)

less picorv32a.synthesis.v
![image](https://user-images.githubusercontent.com/123365348/216235244-8acc6f0e-0a02-4070-b727-eb9b6cf2a160.png)


![image](https://user-images.githubusercontent.com/123365348/216235513-15765fdc-373b-4700-a488-30a704ad926f.png)


# Good floorplanning Vs Bad floorplanning and introduction to library cells

  Configuration openlane
![image](https://user-images.githubusercontent.com/123365348/216237424-afc6d1c2-6fba-4585-96ca-de667ccbed27.png)

less README.md 
![image](https://user-images.githubusercontent.com/123365348/216238078-0cb51d63-4a71-41b2-8eb0-3e2b1fbf6695.png)

less floorplan.tcl


![image](https://user-images.githubusercontent.com/123365348/216238253-d8c74b2d-512a-4705-908a-29ada48373b5.png)


run_floorplan
![image](https://user-images.githubusercontent.com/123365348/216239163-448fad5d-173b-4c13-b9d7-f1499894ef11.png)

less config.tcl

![image](https://user-images.githubusercontent.com/123365348/216251516-4a7979d4-1a92-4ade-b417-e132c0383863.png)

less ioPlacer.log

![imagen](https://user-images.githubusercontent.com/123365348/216531336-f5678d51-216e-4eb9-94ac-7e859fe1d4ff.png)


less sky130A_sky130_fd_sc_hd_config.tcl

![image](https://user-images.githubusercontent.com/123365348/216253043-9900e0af-68bd-4ec9-86ef-5bb1ce278aeb.png)


less picorv32a.floorplan.def
magic -T//home/kaythinzarphu/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.placement.def

![image](https://user-images.githubusercontent.com/123365348/216253351-ba8597a7-4ffc-4c43-9975-b993235ef437.png)

![imagen](https://user-images.githubusercontent.com/123365348/216531405-f505ca71-9ea7-4c37-9b5e-d5699fd8afb8.png)

![imagen](https://user-images.githubusercontent.com/123365348/216531531-ee69f424-dd09-4acf-b7b7-4db5fc387f24.png)

![imagen](https://user-images.githubusercontent.com/123365348/216531575-bae47634-d3e5-4007-9368-75c59eb75e53.png)

The actual layout

![image](https://user-images.githubusercontent.com/123365348/216256295-725a5f3a-003e-44b4-a6aa-442d5e223cf2.png)



%run_placement

![image](https://user-images.githubusercontent.com/123365348/216260263-da98c0f5-d62d-4160-a982-87df62ad1977.png)

magic -T//home/kaythinzarphu/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.placement.def
![imagen](https://user-images.githubusercontent.com/123365348/216531623-e633f429-ddbc-4074-958b-ea5b96095713.png)
![imagen](https://user-images.githubusercontent.com/123365348/216531640-348910e4-7165-4382-bc4b-2a3390153c01.png)






