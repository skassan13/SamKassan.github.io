---
title: "Generative Design SLS Truck Hanger"
excerpt: "SLS electric longboard truck hanger and motor mount using generative design."
header:
  image: assets/img/FrontHangerCrop.png
  teaser: assets/img/HangerCrop.png
gallery1:
  - image_path: assets/img/SKhanger.PNG
  - image_path: assets/img/TopHanger.PNG
  - image_path: assets/img/SideHanger.PNG
  - image_path: assets/img/Hanger.PNG
  - image_path: assets/img/FrontHanger.PNG
  - image_path: assets/img/Hanger.GIF
gallery2:
  - image_path: assets/img/HangerRender.png
  - image_path: assets/img/HangerRenderSK.png


---

# Generative Design and Powder Bed Fusion

Powder bed fusion (PBF) and generative design form a uniquely complementary pairing: PBF gives manufacturers freedom to produce organic, highly optimized geometries that would be impossible with conventional subtractive or casting methods, while generative design provides the computational framework to discover those geometries in the first place. 

PBF is an additive manufacturing method with a market value of over $3 billion as of 2025. A laser or electron beam selectively fuses regions of a powder bed to build parts layer by layer. This enables the fabrication of highly complex, lightweight objects with fine feature resolution and strong mechanical properties. PBF can print both polymers and metals, giving it a wide range of applications.  

Generative design is a novel design approach in which the engineer defines design objectives, constraints, loads, materials, and manufacturing methods, and the software generates optimized structures that satisfy those requirements. Rather than manually shaping parts, designers evaluate and refine computer-generated solutions that often feature organic shapes and reduced volume. 

In practice, the combination of the two technologies has several benefits increases efficiency and reduced manufacturing costs due to the lightweight part designs. Additionally, multi-part assemblies can be consolidated into singular pieces (component interfaces are common sources of failure).  

This combination has found particular success in the automotive and aerospace industries. Recently, engineers from several aerospace companies and universities across the world collaborated to create a lightweight turbine center frame for a large-scale aircraft engine. Commercial aviation is the cause of 2.4% of global carbon emissions, so there has been a strong global push to increase the sustainability of air travel and shipping. Decreasing the weight of the aircraft would increase fuel efficiency and reduce emissions. Using generative design and PBF, the group was able to reduce the 100+ part assembly into one piece, reducing the mass by 30% in the process. 



# Longboard Truck Hanger Design

While the specific object shape is created by the computer, generative design is just as dependent on the user as manual CAD modeling. Generative algorithms only know what you tell them - loads, constraints, preservation regions, obstacle regions, manufacturing limits, and objectives. If those inputs are incomplete or unrealistic, the optimized geometry will look great on-screen and fail in the real world. 

In this project, I used generative design and PBF to create a truck hanger and motor mount for an electric longboard. In setting up the truck hanger, I selected a single fixed structural constraint on the middle kingpin through-hole to represent the part’s attachment to the deck. That placement is physically reasonable because the kingpin/pivot region is where the hanger is clamped to the assembly, and fixing it forces the computer to carry applied forces through the hanger to that connection. 

To decide which forces to apply, I used a combination of mechanics and expected scenarios: static vertical load from rider weight (split between trucks), lateral shear for turning, longitudinal shear for braking, weight of the motor creating a moment against the motor mounting plate, the tension of the belt pulling against the plate, and a moment from the motor’s torque. I placed the vertical, lateral and longitudinal forces at the wheel/axle interfaces because that is where the tire transmits load into the hanger. I added a torsional moment about the pivot to ensure the kingpin region carries realistic twist. I ran separate load-cases to ensure the optimizer met all requirements. 

By creating outcomes using both aluminum and nylon (Nylon12), you can see how the mechanical properties of the material selection impact the generative design process. Aluminum’s stronger mechanical properties result in a lighter, sleeker model with thin trusses and wide gaps between sections, while the nylon model is almost completely filled out. If the aluminum model was printed out of nylon and attached to the board, it would not be able to withstand the applied forces and would break. 

Generative design is extremely useful for discovering non-intuitive load paths that reduce mass while preserving stiffness. It shines in applications where it is unrestricted by traditional manufacturing constraints - this is where the coupling with PBF merges seamlessly. It has found success in the design of aerospace and automotive components, including heat exchangers, engine mounts, and brake calipers. Drawbacks include dependence on accurate loading and boundary conditions and significant computational demands. Additionally, being handcuffed to PBF has its own drawbacks - limited control over surface finish, internal defects in PBF parts, and high manufacturing costs, as PBF is an expensive process. Even if using PBF to print a generative design component decreases weight and increases strength, it may not be financially feasible. 

In short, powder bed fusion and generative design are powerful technological tools for reducing part count and mass, but its success depends on proper load definition, appropriate constraints, and design objectives. With the market value of PBF expected to exceed $3 billion in 2025, we will likely be seeing much more of this combination in years to come. 


{% include gallery id="gallery1" %}

# Aluminum CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811a1743f3bc3bfcbac?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


# Aluminum CAD Renders
{% include gallery id="gallery2" %}
