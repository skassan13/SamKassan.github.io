---
title: "Multi-material Pliers"
excerpt: "Print-in-place FDM pliers made of PLA and TPU."
header:
  image: assets/img/PliersHor.PNG
  teaser: assets/img/PliersHor.PNG
gallery:
  - image_path: assets/img/PencilPickup.GIF
  - image_path: assets/img/PliersClosing.GIF

   
---

# Print-in-place Method
Print-in-place 3D printing enables the fabrication of fully assembled mechanisms - such as hinges, gears, sliders, and compliant joints - in a single manufacturing step. These designs rely on engineered clearances and geometric constraints that prevent adjacent parts from fusing during printing, allowing functional motion immediately after fabrication. This approach eliminates post-printing assembly and is widely used for rapid prototyping, functional mechanisms, and consumer devices such as spring-loaded boxes, and interlocking hinges. 

Print-in-place has been applied across both hobbyist and industrial contexts. Community projects include puzzles, phone stands, compliant hinges, locking boxes, and poseable figurines, while engineering and industry sources highlight functional gear trains, snap-fit enclosures, and SLS-printed fixtures that require no assembly. 

The material and printing method used - FDM, SLA, or SLS - strongly affect print-in-place performance.

* FDM is the most accessible process but requires the largest clearances because of layer lines, material extrusion variability, and stringing. Functional print-in-place parts are typically printed using tougher engineering filaments such as PETG, ABS, or nylon to reduce brittleness, though designers must accommodate increased tolerances and more frequent iteration. FDM does provide an interesting alternative due to its multi-material extrusion capability - an elastic TPU piece can be printed into a rigid model to provide flexibility.

* SLA offers very high resolution, making it ideal for small features, intricate mechanisms, and precise clearances. However, standard resins can be brittle, so hinges and load-bearing components perform better in tougher resins.

* SLS (typically Nylon 12) is often considered the best general-purpose process for strong, functional print-in-place mechanisms. Powder-based printing eliminates the need for support structures and produces uniform parts with excellent dimensional stability and low friction between moving components. SLS nylon is used extensively in industry for snap-fits, living hinges, gears, and integrated assemblies that must withstand repeated motion or mechanical stress.
 
Overall, print-in-place manufacturing combines intelligent mechanical design with the unique capabilities of additive processes to create functional mechanisms in a single print. When paired with the right material and printing method—particularly SLS or engineering-grade SLA/FDM materials—PIP offers a powerful approach for rapid prototyping, educational models, assistive devices, and research tools that require compact, reliable motion without assembly.


# Device Design
The jaws and handles of the pliers were printed out of PLA, with the elastomeric middle region made of TPU. The TPU region flexes when the handles are squeezed, pulling the jaws together. Dove tail joints with .05mm clearances hold the components together without requiring tools for assembly. The jaws are 30mm long with a 10mm clearance.

# Slicer Settings
To achieve the desired level of flexibility in the TPU joint, the infill pattern was changed to a grid pattern. The horizontal top and bottom layers were removed and extra layers around the perimeter were added to reduce flexion in the wrong axis. the infill density was set to 45% and the infill extrusion width was set to 1.2mm - double the 0.6mm nozzle size - in order to increase the strength of the infill lines. These settings may vary depending on the specific device geometry, as multiple iterations were required to achieve the desired functionality. 


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b60281175b72d497c782ac4?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery id="gallery" %}

