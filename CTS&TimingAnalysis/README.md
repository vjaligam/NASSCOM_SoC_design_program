#update readme

Tracks. info screenshot

![image](https://github.com/user-attachments/assets/76b077b3-1ff2-44b0-a93e-7d5ec6e3267f)

![image](https://github.com/user-attachments/assets/7de7e788-ebef-4518-87e6-f64e337f5d05)


Condition1: The input and output ports of the standard cell should lie on the intersection of the vertical and horizontal tracks. 
![image](https://github.com/user-attachments/assets/62dbface-8be1-431c-9a7f-27ff7800b20f)


Condition2: Width of the standard cell should be odd multiples of the horizontal track pitch. 
![image](https://github.com/user-attachments/assets/f2e3b18a-5629-426d-af8a-6e523a9d6513)
1.38um is odd (3) multiple of 0.46um

Condition 3: Height of the standard cell should be even multiples of the vertical track pitch.

![image](https://github.com/user-attachments/assets/68cef70d-ac5c-4dcf-bf33-3a1802667163)

2.72um is even (8) multiple of 0.34um

Save the finalized layout with custom name and open it.
Command for tkcon window to save the layout with custom name

# Command to save as
save sky130_vsdinv.mag
Command to open the newly saved layout

# Command to open custom inverter layout in magic
magic -T sky130A.tech sky130_vsdinv.mag &

Generate lef from the layout.
Command for tkcon window to write lef

# lef command
lef write
![image](https://github.com/user-attachments/assets/2a103142-3e34-4732-8169-1441ba654446)



Copy the newly generated lef and associated required lib files to 'picorv32a' design 'src' directory.
# Copy lef file
cp sky130_vsdinv.lef ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/src/

# Copy lib files
cp libs/sky130_fd_sc_hd__* ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/src/

![image](https://github.com/user-attachments/assets/5cfd918e-d7d3-4e6d-af7e-4ad3d54a8879)


![image](https://github.com/user-attachments/assets/f3918e51-314b-4c93-8c24-2ef7117c4dd0)





