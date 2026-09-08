# A3 – [Topic]

## Objective
- Use axial deflection modeling to design its dimensions
- Use parametric design to determine a bars length
- Introduce you to FEA (Finite Element Analysis)
- Introduce you to linking dimensions to appropriate parameters in CAD.
- Compare and contrast the different analysis

<img width="442" height="107" alt="image" src="https://github.com/user-attachments/assets/fe6a1741-2ac3-41ee-a163-f944d921c44c" />

## Analyze
<img width="2707" height="1270" alt="IMG_0258" src="https://github.com/user-attachments/assets/c429e277-69e4-4a0b-ba28-6c64a278dd56" />

To meet the design requirements for maximum stiffness under direct axial tension, a cylindrical aluminum rod was sized using analytical deflection equations. Given a tensile load of 400lbf, a target deflection limit of 0.009in, and an elastic modulus of 10x10^6 psi, a baseline diameter of 0.50 in. Using this diameter, the cross-sectional area was determined, which was then substituted into the axial elongation relation delta = FL/AE to parametrically solve for the allowable bar length of 44.18 in.

For the CAD portion of the documentation, I chose Creo Parametric due to me having experience in the software. Before drawing a single sketch, I popped open the Parameters menu and entered my baseline values: applied load, target deflection, Young's modulus, and bar diameter. From there, I used the Relations tool to plug in the formulas for cross-sectional area and bar length. This essentially turned Creo into an built-in spreadsheet—it instantly calculated the required length and confirmed my hand calculations were spot on.
CAD Design:
<img width="668" height="407" alt="image" src="https://github.com/user-attachments/assets/63c06e66-d4b1-4fb0-b981-411b08c82d7f" />

With the parameters ready, I sketched a simple circle and tied its dimension directly to my d0 parameter. I then extruded it into a cylinder, setting the length to d1, which automatically pulled from the length formula I set up in the Relations box. Since Creo only lets you assign materials to a 3D model, I went into the Model Properties and assigned Aluminum to the part so the physical properties would update.
<img width="399" height="190" alt="image" src="https://github.com/user-attachments/assets/b3adf904-4e05-421f-abcb-2610f8a9a6d7" />


<img width="529" height="309" alt="image" src="https://github.com/user-attachments/assets/90645cb4-5df6-4b9c-a78f-1671539d0ce7" />

Analysis: 
To run the FEA, I switched Creo over to Simulate mode and fixed the left face of the bar while applying a pulling force to the right end. I tied this load directly to my pre-set "F" force parameter. Once the boundary conditions were set, I ran the simulation and generated both an axial deflection map and a von Mises stress map. The results are shown below, with von Mises stress on top and axial deflection  on the bottom.
<img width="1082" height="404" alt="image" src="https://github.com/user-attachments/assets/b7d82678-fc44-4d48-b612-2e6a5bede68c" />

<img width="1082" height="404" alt="image" src="https://github.com/user-attachments/assets/b6642602-dd7a-4640-8a92-a458be374e9f" />


<img width="2893" height="1705" alt="IMG_0259" src="https://github.com/user-attachments/assets/d89d57d3-f4c1-4658-afde-42f401a025ad" />

After running the simulation and extracting the stress values, the nominal stress from my hand calculations came out to 2.037 ksi, which is well below the 40 ksi yield strength of aluminum. Creo reported a slightly higher peak stress of 2.295 ksi right near the fixed boundary condition, yielding a safety factor of 17.43. The axial deflection from the FEA matched my hand calculations almost perfectly, with only a 1.06% difference which was awesome. This minor variation makes complete sense my hand calculations assume ideal, uniform strain along the entire bar, whereas the FEA accounts for the extra local stiffness created by rigid constraints at the fixed end.

<img width="2498" height="748" alt="IMG_0261" src="https://github.com/user-attachments/assets/859dc189-8719-45e3-be53-988d75cb5c66" />

Using Peterson's Stress Concentration Factors, a standard transverse hole in a tension member gives a theoretical stress concentration factor of Kt = 2.5. Multiplying this by my nominal stress gave a peak stress of 5.10 ksi right at the edge of the hole. Since this peak stress is still way under Aluminum's 40ksi yield strength, the updated safety factor drops to 7.8. Even with the added stress concentration, the design easily clears the yield limit and remains completely safe.

## Decide
Before this project, I had zero experience running FEA on a CAD model, so there was definitely a learning curve. The reason I chose Creo is due to me having it already installed and also past experience. I did run into a minor setup mistake in Creo when I first built the model. I forgot to include the cross-sectional area equation in the Relations box, so my length formula wasn't evaluating correctly and the geometry wouldn't update. Once I realized the missing parameter link, I went back in, added the area relation, and the model instantly scaled to the correct size. The only other point of confusion was the prompt itself: the main description called for a circular cross-section, while the rubric outline mentioned width, height, and thickness like a rectangle. I decided to stick with the circular design, and the results turned out great. Overall, the project took me about 5 hours this past weekend.

## Communicate
Download CAD file: 
https://drive.google.com/file/d/1qs9wgRU30TB8TUcFKbwXSpgg7g1Vj8Rf/view?usp=sharing

