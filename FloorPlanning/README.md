After the synthesis completed, it is now time to start the floorplan.  Before we start the floorplan, let's review some of the files that are used in floorplanning.


Calculate the Die Area from the 


![image](https://github.com/user-attachments/assets/868f30b7-719c-4ac6-85cd-ea0a05260fdf)


1000 units = 1 Micron
Die Width = 660685/1000 = 660.685us
Die Height = 671405/1000 = 671.405us

Die Area = Die Width x Die Height = 660.685us x 671.405us

Opening floorplan in Magic tool:
magic -T /home/vsduser/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.floorplan.def &


![image](https://github.com/user-attachments/assets/e32a5765-1898-4be2-ae68-40d4338d6021)


![image](https://github.com/user-attachments/assets/3af95701-eabc-40a7-bc24-8d7617d032e6)


Standard cells

![image](https://github.com/user-attachments/assets/a3c7c87e-ea06-430a-93f6-c43e76aa5d6e)


Placement:

![Screenshot 2024-09-30 141243](https://github.com/user-attachments/assets/af4a5249-dc91-45ee-a693-8d06e9c12dc8)


![image](https://github.com/user-attachments/assets/ac43d467-0a81-4e11-83a5-c9f2b782f783)


![image](https://github.com/user-attachments/assets/c4d009d7-8ef8-4563-92d8-4fe2e481f181)


  


