# A2 – Truss Stress Analysis

## Objective
Step 1: Truss Geometry
I was given this image with points on it and was challenged with designing a truss to support the loads provided.
<img width="428" height="243" alt="image" src="https://github.com/user-attachments/assets/0d4983a8-dee8-42a2-be3a-c6823cffb302" />

<img width="2370" height="3099" alt="IMG_0169" src="https://github.com/user-attachments/assets/546e3e16-c945-4a76-a742-1c732452200c" />

I chose P to be 25kN, a=0.4m, b=0.3m. Point A is a Pin and point B is a roller. I started by creating a truss geometry. I decided to go with a 7 member truss geometry connecting all the points made from triangles. I had to add a point E that spans halfway between point A and B. After designing my inital design, I began to draw FBD's of the whole structure to then be able to solve for every point and member within the truss. 

<img width="2361" height="1794" alt="IMG_0170" src="https://github.com/user-attachments/assets/067bd33e-87d7-4535-909a-26faca34a014" />

I found that the diagonal distances between the members. I then found that my largest force to be 27.778kN. Next to find the cross sectional area of the beam I needed to use known factors of the material, A500 Steel, such as its density, yield strength, safety factor, and max forces. I used these to find the cross section and the estimated weight of the truss. I will circle back to weight in the CAD section.


## Analyze
Step 2: Pin Calculations
To calculate the pin cross-sectional area and estimated weight for a single shear setup, I used the governing force, safety factor, material density of tool steel, and shear strength. To simplify the force analysis, I drew a free-body diagram for pin D and combined vectors P and DC into a single force, F1. Since the system is in equilibrium Sum F=0 and F1 equals FA, I was able to reduce the four acting forces down to just two.

However, early in the process, I accidentally applied the factor of safety a second time, which threw off all my subsequent area and weight values. Overlooking this mistake, I wrongly assumed the error came from using a single shear approach. Against the assignment instructions, I switched to a double shear setup, which messed up the numbers even more. It wasn't until I started modeling the components in CAD that I caught the original error and had to clear out and redo the calculations.

<img width="2504" height="1696" alt="IMG_0172" src="https://github.com/user-attachments/assets/ab4bbf17-e3ef-4939-8f22-e3990546b941" />

## Decide
Step 3: CAD design

<img width="850" height="293" alt="image" src="https://github.com/user-attachments/assets/ecf4e902-5dc5-4027-9ada-4e34af85ed36" />


<img width="2523" height="957" alt="IMG_0173" src="https://github.com/user-attachments/assets/4e6079b5-ca0e-4675-8019-85b81f7ac826" />


<img width="668" height="398" alt="image" src="https://github.com/user-attachments/assets/a9c7354b-d570-4af9-9912-66e2ed86584d" />
The Pin
The connecting pins were modeled as solid cylindrical components extruded from hardened tool steel to handle the single-shear loads at Nodes A through E. Each pin features a diameter of 11.0 mm to provide the required cross-sectional area of 94.8 mm², paired with a length of 20.0 mm to match the full thickness of the truss plate. The CAD simulation calculates the weight of a single pin at approximately 0.032 lbs (0.143 N), resulting in a combined assembly weight of 0.161 lbs (0.716 N) across all five joints, which exactly matches the theoretical weight derived in the hand calculations.
<img width="1101" height="566" alt="image" src="https://github.com/user-attachments/assets/6a1378d0-1d89-41e8-a183-896059b8e204" />
The 7-member planar truss was modeled in CAD as a single continuous 20.0 mm thick plate with internal triangular cutouts and integrated node connection points, matching the design layout from Appendix B. Each member features a uniform cross-sectional width of 16.8 mm to satisfy the calculated minimum required area of 335.3 mm², spanning an overall base length of 1.0 m. The CAD mass properties analysis yielded a simulated weight of 18.8 lbs (83.6 N), which compares favorably against the hand-calculated theoretical weight of 20.9 lbs (92.95 N). The roughly 10% reduction in the CAD model accounts for material removed by the five 11.0 mm pin holes and the geometric overlap at the intersecting joint nodes, whereas the hand calculations assumed full center-to-center member lengths without joint deductions.

_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

