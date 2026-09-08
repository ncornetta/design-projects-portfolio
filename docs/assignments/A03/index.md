# A3 – [Topic]

## Objective
- Use axial deflection modeling to design its dimensions
- Use parametric design to determine a bars length
- Introduce you to FEA (Finite Element Analysis)
- Introduce you to linking dimensions to appropriate parameters in CAD.
- Compare and contrast the different analysis

<img width="442" height="107" alt="image" src="https://github.com/user-attachments/assets/fe6a1741-2ac3-41ee-a163-f944d921c44c" />

## Analyze
To meet the design requirements for maximum stiffness under direct axial tension, a cylindrical aluminum rod was sized using analytical deflection equations. Given a tensile load of 400lbf, a target deflection limit of 0.009in, and an elastic modulus of 10x10^6 psi, a baseline diameter of 0.50 in. Using this diameter, the cross-sectional area was determined, which was then substituted into the axial elongation relation delta = FL/AE to parametrically solve for the allowable bar length of 44.18 in.

For the CAD portion of the documentation, I chose Creo Parametric due to me having experience in the software. Before drawing a single sketch, I popped open the Parameters menu and entered my baseline values: applied load, target deflection, Young's modulus, and bar diameter. From there, I used the Relations tool to plug in the formulas for cross-sectional area and bar length. This essentially turned Creo into an built-in spreadsheet—it instantly calculated the required length and confirmed my hand calculations were spot on.
CAD Design:
<img width="668" height="407" alt="image" src="https://github.com/user-attachments/assets/63c06e66-d4b1-4fb0-b981-411b08c82d7f" />

I used these equations to set the parameters 

<img width="399" height="190" alt="image" src="https://github.com/user-attachments/assets/b3adf904-4e05-421f-abcb-2610f8a9a6d7" />

<img width="529" height="309" alt="image" src="https://github.com/user-attachments/assets/90645cb4-5df6-4b9c-a78f-1671539d0ce7" />

Analysis: 
<img width="1082" height="404" alt="image" src="https://github.com/user-attachments/assets/b6642602-dd7a-4640-8a92-a458be374e9f" />


## Decide


## Communicate

