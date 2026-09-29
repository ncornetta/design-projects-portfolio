# A6 – [Topic]

## Objective
As part of this assignment, a complete solid model and multi-view engineering drawing will be created to accurately represent the bracket designed in Project A5. The model will include all necessary features and dimensions to ensure that the bracket satisfies both the required strength and stiffness criteria. The design will continue to use aluminum as the selected material, with a safety factor of 4 and an applied load of 600 lbf.

## Step 1: Strength vs Stiffness

Before beginning the modeling and drawing process, the first step was to determine which analysis-based design would be used for the final bracket. I selected the strength analysis design because it provided more substantial dimensions while still meeting the required performance criteria. Compared with the stiffness analysis design, the strength-based design resulted in a generally thicker and more robust bracket, especially in features B and D.

After selecting the final design, I opened Creo and began setting up the model. Aluminum was assigned as the material, and the unit system was set to inches and pound-force (in/lbf) before beginning the solid modeling process.


<img width="487" height="242" alt="image" src="https://github.com/user-attachments/assets/704ee97b-2853-415e-af42-549079be2882" />


<img width="261" height="310" alt="image" src="https://github.com/user-attachments/assets/04a1bf1a-a132-4e88-ad7f-db6260e7dfbb" />


## Step 2: Parametric Modeling


Using Creo, I created a single solid part by developing a series of continuous sketches, beginning with Feature A and working through Feature E. This approach allowed me to visualize the overall geometry of the bracket and determine how the selected dimensions would work together in the final model. During this process, I identified a few dimensions and assumptions from my original design that needed to be adjusted.

The original height of Feature B was set to 1.00 in., but it was increased to 1.25 in. to provide additional clearance between features without negatively affecting the overall design. Feature D was originally given a height of 1.60 in., but this was reduced to 1.50 in. after recognizing that I had overestimated the required dimension in my previous A5 design.

Once these adjustments were made, I entered the finalized dimensions into Creo Parameters and created the necessary relations to control the dimensions throughout the model. This allowed the bracket to be fully parametric and made it easier to manage any future dimensional changes. Below is a series of images showing the order of operations used to create the final model.







Step 3: Tolerances and Drawing

To ensure that the part met the required design specifications, I reviewed the model and applied the appropriate tolerances and significant figures to each feature. After confirming that all dimensions and tolerances were correct, I created a B-size engineering drawing using the format provided by UNCC.

While setting up the drawing in Creo, I found that the tolerance values were not displayed automatically. To correct this, I went into the configuration settings and manually enabled the proper tolerance display options. Once the settings were adjusted, I completed the engineering drawing with all necessary dimensions and tolerances.

The final drawing includes a 3D orthogonal view of the bracket along with top, front, and right-side views. These views clearly display the part geometry, dimensions, tolerances, and hidden features needed to fully represent the final design.

Reflection:
I spent approximately six hours completing this assignment, and one challenge I encountered was making sure the parameters and relations in Creo updated the model correctly without causing conflicts between dependent dimensions. The diameter of Feature A was determined using the strength analysis by combining the allowable stress and section modulus equations, and this dimension was then used to control the width of Feature B, while its thickness was calculated through the Creo relation d5 = (4*1200)/(40000*DA). Feature D was given a loose-fit tolerance of -0.001 in. to create a functional sliding interface that allows the bracket to move freely along the mating component while still maintaining a secure fit. This assignment also demonstrated the importance of selecting reasonable tolerances, since unnecessarily tight tolerances, such as 0.0001 in. instead of 0.001 in., can significantly increase manufacturing time and cost by requiring greater machining precision.
## Decide


## Communicate

