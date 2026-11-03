# A8 – Gears

## Objective
- Design a gearbox that can be assembled and disassembled.
-  and size input and output shafts for strength.
- Design journal bearings to support shafts.
- Create a gearbox housing with proper clearance and fastening.
- Use parametric CAD modeling to generate a final design.
- Document calculations, sketches, and lessons learned.

Description:

Design a gearbox which can be assembled and disassembled. The spur gears have a gear ratio of 24:9 and are listed in the resource section. The output gear torque and speed are to be 1.25 in-lbf and 1100 rpm relative. The input (pinion,power-transmission) and output (gear, short shaft) shaft diameters are .125 and .25 inches respectively and each have a length of 1 inch. Use the appropriate equations in the Machinery’s Handbook for empirical units. The critical features of the gearbox include the shafts, and the journal bearings.

Assumptions:

-  appropriate strength of shafts, use Machinery’s Handbook.
- The gear train is ideal.
- The moment of the radial force from the gear train is small enough to be ignored.


<img width="464" height="325" alt="image" src="https://github.com/user-attachments/assets/5f5f407e-0b3a-401a-b109-f4a75ce9978a" />



## Shaft Design

To design the input (power-transmission) and output (short) shafts, I first gathered the formulas needed to determine transmitted power, applied torque, and rotational speed. Utilizing the 24:9 gear ratio enabled me to solve for both torque and speed. The power equation was sourced from the Machinery's Handbook, incorporating maximum allowable shear stresses of 4,000 psi for the input shaft and 8,500 psi for the output shaft. From these relations, I computed the required shaft diameters based on power and torque constraints. Because the resulting dimensions fell safely within acceptable limits, no modifications to the original shaft diameters were necessary.


<img width="393" height="526" alt="image" src="https://github.com/user-attachments/assets/70ec38cb-bd2c-4f85-8475-1125557dace9" />


Journal Bearing Design:
To select the correct journal bearing from the McMaster-Carr catalog, we first needed to determine the appropriate material and wall thickness. Selecting the right material involved calculating operating pressure, velocity, and the corresponding PV rating.

Assuming an initial bearing length of 1/4 inch and designing for running/sliding fits, I used the RC5 fit table to establish the inner diameter for both shafts. From these calculations, I evaluated the PV metrics and determined that dry graphite was the optimal material choice.

The final step in the design process was calculating the bearing thickness using the pressure/axial stress formula. By applying the radial force to the cross-sectional area of the bearing diameter, I successfully derived the required thickness for each component.


Calculations and also thickness

<img width="394" height="527" alt="image" src="https://github.com/user-attachments/assets/37f20bfc-3c03-4379-a084-95bff7909819" />






## CAD Design

Because McMaster-Carr provided downloadable CAD models for the gear, pinion, and journal bearings, my design work focused primarily on the shafts and housing. The shafts were modeled using the specified diameters and lengths, incorporating chamfers to facilitate the press-fit assembly. For the housing, I utilized the dimensions of the internal components to create a compact and secure enclosure. When evaluating fastening options, I chose a snap-fit design over a traditional bolted configuration; given the miniature size of the gear and pinion, bolting would have been excessive and inefficient regarding manufacturing material usage. Once all components were modeled, I integrated them within SolidWorks Assembly. To properly simulate the gear interaction, I applied a mechanical gear mate corresponding to the 24:9 ratio. All modeling and dimensions within SolidWorks were maintained in Imperial units (inches).


Input Shaft

<img width="451" height="272" alt="image" src="https://github.com/user-attachments/assets/6e8dd124-72bc-49b6-9b8a-8253918087d0" />


Output Shaft

<img width="341" height="262" alt="image" src="https://github.com/user-attachments/assets/91dfcfa9-bea7-43b5-8275-2b5985243ac7" />

Drawing
<img width="344" height="423" alt="image" src="https://github.com/user-attachments/assets/ff274c64-25c1-46a3-a3fd-d81e59e5e616" />



<img width="443" height="316" alt="image" src="https://github.com/user-attachments/assets/f2c6af4a-f047-45c2-b278-0ced73df800c" />



<img width="164" height="260" alt="image" src="https://github.com/user-attachments/assets/f13cbed3-954c-4423-9462-73937b77a7d1" />




<img width="274" height="274" alt="image" src="https://github.com/user-attachments/assets/14f82861-4dca-4c0a-827e-4872ed2d4eaa" />




<img width="439" height="341" alt="image" src="https://github.com/user-attachments/assets/caae3515-ed2c-42ef-86b3-28d399757f9a" />




## Lessons Learned
Overall, the project took about eight hours to complete, with the majority of that time spent working in SolidWorks. The biggest learning curve involved navigating SolidWorks itself; because McMaster-Carr did not offer compatible downloadable models for the gear, pinion, and bearings in Creo, I had to switch to SolidWorks. Having not used the software since high school, I was quite rusty, which led to some initial challenges during the assembly phase. This experience highlighted the importance of becoming more proficient in SolidWorks, given its widespread industry adoption. Beyond software familiarity, I gained valuable practical skills, such as calculating bearing thickness when an outer diameter is not provided. I also continued to appreciate the immense value of the Machinery's Handbook; learning to navigate and reference it efficiently will undoubtedly serve as a critical tool throughout both my academic and professional career.

Cad Files:
https://drive.google.com/file/d/10WRvS7nGjJmj7On4xiF2WVsdsZHoZii4/view?usp=sharing
