---
title: "Generative Design SLS Truck Hanger"
excerpt: "SLS skateboard truck hanger and motor mount using generative design."
header:
  image: assets/img/BikeMountVert.png
  teaser: assets/img/BikeMountVert.png
gallery1:
  - image_path: assets/img/PhoneHoldHor2.png
  - image_path: assets/img/PhoneHoldVert.png
  - image_path: assets/img/PhoneHolder.GIF
gallery2:
  - image_path: assets/img/PhoneRender2.png
  - image_path: assets/img/ClampRender.png
  - image_path: assets/img/Detent.png
  - image_path: assets/img/Swivel.png
  - image_path: assets/img/DetentFull.png
  - image_path: assets/img/PhoneSlot.png

---

# Top Down Modeling

Top-down modeling is a CAD design strategy in which the overall system layout and critical reference geometry are created first, and individual components are then designed in context around those references. Rather than modeling parts independently and assembling them afterward, top-down modeling uses shared geometry, projected sketches, and in-place features so that all components fit together precisely and update predictably when changes occur. This approach is especially effective for multi-component mechanisms where clearances, alignment, and interfacing surfaces must remain tightly controlled.

In this project, top-down modeling is the foundation for designing a functional phone holder that clamps to a bike handlebar and allows tool-free rotation between portrait and landscape orientations. The project begins by creating the handlebar as the first component. This establishes a fixed, accurate reference for both the clamp mechanism and the viewing orientation of the phone. Anchoring the handlebar ensures that all subsequent components are positioned relative to a stable datum, preventing misalignment as the design evolves.

Overall, top-down modeling enables a more controlled, adaptable, and assembly-aware design process. By using shared reference geometry and in-context features, I designed a multi-part, functional phone holder that rotates smoothly, snaps into place, and mounts securely to the handlebars.

# Bike Phone Mount Design

The clamp and detent mechanism were printed in PLA because these parts require rigidity and dimensional stability. Using PLA kept the rotation mechanism consistent and prevented deformation that could weaken the detents over time. 

The phone-holding component, however, was printed from TPU. Its flexibility allows the phone to snap securely into place without tools. TPU also improves grip and absorbs vibration, helping it stay locked in during a bumpy ride.

Instead of using a single spring-loaded ball bearing for the detent, the design incorporates four evenly spaced around the circular rotation pieces. This multi-detent layout provides smoother, more stable rotation. With four detents, the phone clicks firmly into both portrait and landscape orientations and resists wobbling or unintentional movement.

M3 and M5 heat set inserts were added to attach the components. The clamp requires two M5 screws - one on each side - to secure the mount to the handlebar. While an allen wrench is required for initial assembly and attachment of the phone mount, no tools are required for placement, rotation, or removal of the phone.

{% include gallery id="gallery1" %}

# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811553ac4e0d2a931ca?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


# CAD Component Renders
{% include gallery id="gallery2" %}
