# A4 – [Topic]

## Objective
<img width="298" height="190" alt="image" src="https://github.com/user-attachments/assets/c778d7de-1238-4b7b-8391-0f84ab7560d1" 
  <img width="665" height="266" alt="image" src="https://github.com/user-attachments/assets/886da5dc-6a7d-4ae4-8d2b-543c88f3b68b" />
The objective of this assignment is to design a structural motor mount that securely attaches a 24V DC planetary gear motor to a rigid vertical wall under a 300 N applied shaft load. Rather than relying solely on intuition or CAD, this project bridges theoretical mechanics with practical mechanical design. It requires evaluating structural failure under two distinct design limits: yield strength and maximum allowable deflection, to determine which mechanism governs the geometry.

<img width="380" height="502" alt="image" src="https://github.com/user-attachments/assets/98ec5f3a-48bc-45db-97e5-662835de3e09" />
To model the mount using structural mechanics, the individual plates were decoupled and analyzed separately as cantilever beams according to the procedures in Appendix B. The joint between the two sections and the four-bolt attachment to the overhead surface were modeled as fixed supports, whereas the extended segment along Wall A was treated as flexible under bending. Similarly, when evaluating Feature 2 as a cantilever, the interface connecting Feature 1 and Feature 2 was assumed to act as a rigid boundary for Feature 1.

Furthermore, the analytical model treats Wall A as infinitely stiff, providing rigid restraint for the mounting hardware, while omitting the self-weight of the motor to concentrate entirely on the primary external load path. Finally, the chosen safety factor of 3 is assumed to absorb local stress concentrations surrounding the center shaft opening and the 3.4 mm fastener clearance holes.

PLA was chosen as the optimal material from the options listed in the assignment, primarily due to its superior stiffness (Elastic Modulus). Drawing from verified material data on MatWeb, a tensile yield strength of 45.2 MPa was selected to guarantee structural integrity under load, while a mean elastic modulus of 2,350 MPa was applied to model part rigidity accurately. Because high stiffness is critical for controlling total component thickness, maximizing the material's baseline elasticity was essential for this design.

<img width="972" height="949" alt="IMG_0320" src="https://github.com/user-attachments/assets/2661ef15-c528-4cba-b11d-98500e78fbb9" />

<img width="1408" height="1081" alt="IMG_0320 (1)" src="https://github.com/user-attachments/assets/874eeee3-1956-44bb-945b-1e5cb7377492" />

<img width="407" height="129" alt="image" src="https://github.com/user-attachments/assets/e5413c7d-1ed3-478b-82b0-01fb81789437" />

<img width="2115" height="825" alt="IMG_0320 (2)" src="https://github.com/user-attachments/assets/e21d2dbf-8b3d-4a83-ad15-e9483f302433" />
As illustrated in the figure below, calculating the allowable stress from the MatWeb yield strength and the target factor of safety yields an allowable stress of 15.07 MPa.
The second figure highlights the hatched cross-sectional area of Feature 1, establishing the orientation used to define the section's width and thickness.
Finally, the standard area moment of inertia equation for a rectangular cross-section is applied, which feeds directly into the subsequent flexure formula calculations.

<img width="2240" height="711" alt="IMG_0320 (3)" src="https://github.com/user-attachments/assets/a81f33a3-ce78-4c3e-966c-e74a2f910077" />

As depicted above, the flexure formula incorporates the internal bending moment derived from FBD 1 alongside the area moment of inertia for Feature 1. Expressing the moment of inertia in terms of the section thickness allows us to isolate and solve for that specific dimension.
Evaluating the relationship both symbolically (Eq. 1) and numerically yields a minimum required thickness of 8.47 mm to satisfy the allowable stress constraint.

<img width="2235" height="1010" alt="IMG_0320 (4)" src="https://github.com/user-attachments/assets/d84a569c-76f1-4968-bc02-f46d674be071" />

Having evaluated the section thickness based on allowable stress, we must next evaluate the potential governing thickness using the maximum deflection constraint specified in the problem.

The beam deflection formula directly incorporates the area moment of inertia, enabling us to isolate the thickness variable once again. Solving both symbolically and numerically reveals that meeting the deflection limit requires a minimum thickness of 15.65 mm.
Because this value exceeds the stress-based dimension, it becomes the governing thickness, representing the true minimum dimension needed to satisfy all design constraints.

Feature 2
<img width="281" height="188" alt="image" src="https://github.com/user-attachments/assets/4ea75601-6906-41ee-8662-273e83026a66" />
<img width="257" height="126" alt="image" src="https://github.com/user-attachments/assets/f025b001-e5ef-42a6-afa0-804f89dce3bd" />
For Feature 2, the given parameters include an applied shear load of 300 N transferred directly from Feature 1 and a resulting bending moment of 24,000 N-mm at the wall interface. The selected material is PLA, which features a tensile yield strength of 45.2 MPa and an elastic modulus of 2,350 MPa. Applying the target factor of safety of 3 yields an allowable stress limit of 15.07 MPa, while the maximum allowable tip deflection is constrained to 0.30 mm. The wall interface is anchored using four M3 bolts requiring 3.4 mm clearance holes, and Wall A is assumed to act as an infinitely rigid boundary condition with zero slope and zero displacement at the support points.

As demonstrated in FBD 1 and the structural layout below, Feature 2 extends horizontally, using the upper interface as the fixed connection to Wall A.
In FBD 2 directly following the calculations, the motor profile is outlined based on the Appendix A specifications. These geometry constraints offer a secondary approach for determining the complete length of Feature 2, which fully integrates the thickness of Feature 1.
Calculating total length requires summing the motor housing depth, the gearbox body length, and the thickness of Feature 1, which results in an overall length of approximately 91 mm. This final dimension is rounded to simplify downstream fabrication.
With total length established, this value is combined with the shaft length to determine the full moment arm. Applying this total length to solve for the bending moment on Feature 2 yields a value of 32,700 N mm.


<img width="2188" height="569" alt="IMG_0326" src="https://github.com/user-attachments/assets/9f1b8934-6559-4d95-b553-c4008d3630fc" />

<img width="2422" height="1057" alt="IMG_0327" src="https://github.com/user-attachments/assets/426b7ba6-f9e9-4c6c-9402-8e47289a331a" />



## Analyze


## Decide


## Communicate
A major issue that I had during this project was that my wifi went out the day before the due date. This was a major issue as I was not able to complete the project fully in time on the website. I did however finish the cad model but ran out of time to finish uploading all of my work onto the website. 

CAD File:
https://drive.google.com/file/d/1WNoDz6KQjyqb2BfdaKqZD8YgHzmQkVyz/view?usp=sharing
