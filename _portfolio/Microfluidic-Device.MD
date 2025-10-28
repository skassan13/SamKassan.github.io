---
title: "Microfluidic Device"
excerpt: "50x75mm PDMS device designed to separate particles of different sizes."
header:
  image: assets/img/microfluidic-device.PNG
  teaser: assets/img/microfluidic-mold.PNG
gallery:
  - image_path: assets/img/microfluidic-device.PNG
  - image_path: assets/img/microfluidic-mold.PNG

   
---

# Pinched Flow Fractionation
Pinch Flow Fractionation (PFF) is a passive microfluidic technique used to separate particles based on size by exploiting laminar flow. In a PFF device, two streams - a particle mixture and a particle-free buffer - merge at a narrow “pinched” segment. The buffer flow squeezes the particle stream against one wall. 

As the channel widens downstream, laminar flow lines allows the streams of particles to uniformly diverge, with the displacement of the particles varying by size: smaller particles are forced closer to the wall while larger particles remain closer to the center. This allows particles of different sizes to be collected through separate outlet channels without the need for external forces such as electric or magnetic fields. The locations of the separated particles are calculable given the particle diameter, the width of the pinched section, and the width of the broad section.

PFF is valued for its simplicity, continuous operation, and high throughput, making it useful in applications such as cell sorting and blood plasma separation (Ashrafizadeh et al., 2025).

# Device Design

*  **Resin printed mold:** A negative mold of the device was constructed in Fusion360 and printed in clear resin using the Formlabs Form 4 SLA printer.
* **Outlet locations:** The device has 3 outlets - one for the buffer, one for the large particles (425-500μm), and one for the small particles (125-150μm). The spacing of the outlets was determined using the PFF algebraic relationship between device size and particle diameter.
* **Device Geometry:** The buffer outlet receives 62.5% of the liquid, with the rest split evenly between the two other outlets. Thus, serpentine paths were added that give 3.33x higher resistance to the particle receiving outlets, providing proportional resistance in order to ensure a proper flow distribution.
* **Parylene Coating and PDMS Casting:** Before the PDMS cast is created, a parylene coating is added to the resin mold. This prevents uncured resin monomers from leaching out of the mold and interfering with the PDMS crosslinking process.

# Limitations and Future Directions
The outlets feed the streams into barbs with plastic tubing, creating a high variable resistance that changes with the positioning of the tubes. High on-chip resistance was added to each path in order to counteract the downstream effects. Future designs could design a device to hold the tubes in the same position, mitigating the issue.


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811f2a72c55785eb70f?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery id="gallery" %}


# Sources:

Ashrafizadeh, S. N., Zare, M., Khatibi, M., & Ashrafizadeh, S. N. (2025). *A Comprehensive Review of Pinch Flow Fractionation in Microfluidics: From Principles to Practical Applications.* *Chemical Engineering and Processing – Process Intensification*, 208, 110087. [https://doi.org/10.1016/j.cep.2024.110087](https://doi.org/10.1016/j.cep.2024.110087) 

