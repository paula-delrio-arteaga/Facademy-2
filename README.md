# Fabacademy-2
Micro challenge 2
## PHOTOBIOREACTOR

### CONCEPT

Photobioreactor hosting our algae cultures to help them grow. 

### PURPOSE

We wanted to explore the properties of algae for different individual purposes so we decided to start collaborating in the creation of the habitat for its propagation. Once we understand the species then we can be able to collaborate with them in order to develop other projects. We are interested in co-creating with algae and exploring their bioremediation abilities. After gathering enough algae we can then transform it into either food, materials, energy, biofuel, art and other individual purposes. 

### PLANNING AND EXCECUTION

We started by defining the needs of our algae and how many cultures we wanted to have. We decided to start with spirulina. We ordered the spirulina and while it arrived we started researching what we needed in order to keep it alive and help it grow. We got a manual which we are attaching in the files. From this we were able to make a list of the things we needed for cultivating the spirulina. We also reserached how the electronics would work and what parts we needed to get. After having in mind all the components neeeded then we could figure out how the design could look like. 

![spirulinalove](/Images/pbr7.jpg)

Now we started designing how will the spirulina be displayed and how would it work. The tricky part in this was integrating the electronics into the stand for the spirulina. Needing them to be sort of close but also protected in case of any spills.

At first we wanted to create a base box that would hold the 4 bottles of spirulina we wanted to have, one for each of us. The design was intended to have the electronics in the box with the led lights facing upwards to the spirulina. We wanted to do the box with cnc and add some curves which would be done with milling so it would add a more organic aesthethic to it. 

![boxcurvessketch](/Images/sketch1.png)

After discussing it we realised it would take a lot of time to fabricate and we would also have a lot of kerf. After assesing this and seeing more options we decided to change the design into something that would make more sense with an organic structure around the spirulina. So we decided to test this and start sketching some ideas. When we finally agreed on a design we divided by tasks. 

![sketchstand](/Images/sketch5.jpg)

#### CNC

  -Paula B started making the 3D model and plans of the curves that would be fitting below the hung spirulina bottles. Pippa 3D modelled the electronics box in which we were going to place the power, pumps, arduino and the cables. We decided to cut it in 15mm plywood. We cut 2 pieces and added a 5mm pocketing in which the LED lights would pass through, so when we glued both pieces together we could have a 1 cm rail. 
  
  -After setting up the file in rhino, we used the rhinoCam plug in and generated the code for the CNCing. We started by setting up a box which would be the material we selected and the dimensions of it. We used a board of 1200x2400x15.6 aprox. We then defined which curves would be an outer cut, inner cut and pocketing.
  
  -We also created the tool specifications, we used a Flat Mill of 6mm. We had to add the bridges in some of the pieces so they would stay in place and add the file of the screws. After defining all the settings we were ready to export the code. The screws file was exported individually and the rest of the layers were exported together. 
  
  -Once we had the nc code we went to the machine, we put out glasses, hair tie and ear cuffs on (safety first). 
  
  ![safetyfirst](/Images/pbr31.jpg)
  
  -We cleaned the bed of the cnc of any extra material left from before, we placed our plywood sheet and aligned it to the borders of the bed. Then we calibrated the z axis with the button of the cnc. So we placed the button below the tip of the CNC and calibrated it. After getting that ready we opened our file in the computer and ran the screws file. 
  
  -After the marks for the screws were done we moved the head of the CNC in order to get on top and screw. 
  
  ![screwingplywood](/Images/pbr23.jpg)
  
  -Once the material was already screwed onto the bed we were able to run the rest of the file. Our file took about 1:20.
  
  ![cnccut](/Images/pbr4.jpg)
  
  -When the machine was done, we moved the Z axis up and moved it back so we could check if all of the cuts were done properly. After we made sure they were, we went on the bed to take out the screws and remove our pieces and the rest of the material.
  
  ![bedtakingout](/Images/pbr6.jpg)
  
  -*We first had only the curves in the file and we realised we put the pocketing all the way through so we had to stop the machine and cut again but moving our pieces so it wouldn't intersect with the new cut. After cutting the curves we added the files of the box. 
  
  -Postprocessing: After getting all the pieces out, we started sanding them to remove excess bits and leave the piece smooth for assembling. 
  
  ![sanding](/Images/pbr22.jpg)
  
  -Once the curves were ready we were able to glue them together. We applied a thin layer of glue and then used the clamps to hold it together while the glue was doing its job.
  
  ![curveglue](/Images/pbr21.jpg)
  ![curveclamping](/Images/pbr20.jpg)
  
#### 3D PRINTING

  -Marina and Pippa prepared the 3D files for 3D printing. 
  
  -Understanding first the pieces needed and their functions. When the type of joineries were defined we started measuring the dimensions of the material they would be attached to in order for them to fit correctly.
  
 -After making the 3D model we went to the machines to start setting up the file in CURA and PRUSA in order to send them to the machines. We used PLA in white and black for different pieces. We did some tests before and then we were ready to start 3D printing. The parameters we had were 210 heat of the nozzle and 60 heat of the bed. The longest print took 14 hours. 
 
 -We ran five machines at the same time in order to make better use of our time. 
 
 -When the printing was done we had a bit of a struggle to take out the material because it got stuck to the bed. We used the spatula to scrap them off and after some struggle they came out. 
 
 -We spent some time taking out the extra filaments for support and sanding a bit some parts. Then we were able to assemble them for the stand. 
 
 ![3dprinting1](/Images/pbr26.jpg)
 ![3dprinting2](/Images/pbr19.jpg)
 ![3dprinting3](/Images/pbr27.jpg)
 ![3dprinting4](/Images/pbr28.jpg)
 
 #### ELECTRONICS
 
  - Figuring out all the connections to the power supply since we have an Air Pump of 220v, a peristaltic Pump of of 12v and a LED strip of 12v plus our microcontroller ESP32 feather to controll the timing of each component. 
  - We thought we could use the power supply (12v 1A) from the LEDs to also connect the peristaltic pump since it has the same voltage. But after checking how many ampers each component needs, we decided to swith all the connections to a bigger power supply of 12v with 16.5 Ampers. In case we need to scale the project we would be able to connect more pumps to the same power supply. The LED requieres a 0.85 Ampers and the peristaltic pump 0.2 Ampers. 
  
  -
  
  -
  
  -
  
  -
 
 ![boxcurvessketch](/Images/pbr15.jpg)![boxcurvessketch](/Images/pbr11.jpg) ![boxcurvessketch](/Images/pbr12.jpg) ![boxcurvessketch](/Images/pbr14.jpg) ![boxcurvessketch](/Images/pbr9.jpg) ![boxcurvessketch](/Images/pbr10.jpg) ![boxcurvessketch](/Images/pbr13.jpg) ![boxcurvessketch](/Images/pbr17.jpg) ![boxcurvessketch](/Images/pbr18.jpg)
 
 #### LASER CUTTING
 
  -We decided to laser cut an acrylic lid for the electronic box the have electronics visible. 
  
  -Marina prepared the file in rhino and inserted the GROW LAB text for it to be engraved. Once it was done we opened the file in the computer, calibrated the laser cutter with the tool. Chose our material and moved the laser to where we wanted it to start cutting. After this then we put the parameters for acrylic and the type of cut and we sent the job. 
  
 ![acryliccut](/Images/pbr25.jpg)
 
 #### 3D SCANNING
 
  -We wanted to test the 3D scanning tools so we chose to use it to 3D model the neck of the bottles we would use in order to fix them to the rail. 
  
  -As the bottle is clear we then had to tape it around so the phone was able to identify the volume and scan it. 
  
  -This was a bit complicated and in the end the redult was not desirable and we went back to just measuring the different diameters in the bottle neck. 
  
  ![3dscanbottle](/Images/pbr30.jpg)
  
 #### ASSEMBLING
 
  -After having all our pieces together it was time to assemble them together. We started by trying to fit them and making adjustments like sanding or drilling in case they didn't fit perfectly and then put everything we had into place. 
  
  ![assemblingrack](/Images/pbr29.jpg)
  

### SYSTEM DIAGRAM (FUNCTION, PARTS, RELATIONS)

![hangingbottlestand](/images/sketch7.jpg)

![bottlehugger](/Images/sketch6.jpg)

### DESIGN ELEMENTS (HOW YOU DESIGNED IT)

### DESIGN AND FABRICATION FILES

### BOM (BUILD OF MATERIALS) 

### CODING LOGIC (ALGORITHMS AND FLOWCHARTS, PSEUDOCODING)

### PHOTOS OF FINAL PRODUCT


### ITERATION PROCESS (PROBLEMS AND SOLUTIONS)

- We struggled first to find a design that could fit our necessities, the algae's and the electronic's. In this case we prioritised figuring out the electronics first and then seeing how we would connect them to the design.

-Our idea at some point was to CNC 

### FUTURE DEVELOPMENT OPPORTUNITIES

### LINKS TO INDIVIDUAL PAGES
