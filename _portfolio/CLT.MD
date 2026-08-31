---
title: "Central Line Placement Trainer"
excerpt: "Surgical training model for the central line placement procedure."
header:
  image: assets/img/CLTWhole.png
  teaser: assets/img/CLTWhole.png
gallery1:
  - image_path: assets/img/MoldHorizontal.PNG
  - image_path: assets/img/Prongs.png
  - image_path: assets/img/Gel.png
gallery2:
  - image_path: assets/img/CLTbase.PNG
  - image_path: assets/img/CLTWhole.png


---
*Designed in collaboration with Dr. Felix Rozenberg (Internal Medicine, North Shore University Hospital)*

## The Problem
Central line placement is a common but high-risk procedure, and hospitals rely on physical training models to let residents and physicians practice the technique under realistic conditions before performing it on patients. The lab's existing trainer, however, had two significant drawbacks. First, the model was built around a full head bust, making it bulky and impractical to store, transport, or use in a typical training session. Second, and more critically, the mold used to cast the ballistic gel neck piece relied on lengths of tubing threaded through the gel to form the jugular vein and carotid artery canals. Once the gel was cast around the tubing, the tubing itself became a permanent, non-reusable part of the model - meaning every single training session consumed an entirely new set of tubing. This made the trainer repetitive to fabricate, time-consuming to prepare, and wasteful in both material and lab time.

Dr. Rozenberg tasked me with redesigning the trainer to solve both problems: shrink the physical footprint of the model, and eliminate the need to sacrifice a new set of tubing for every use.

The previous trainer that this design is based on can be found here: https://www.aliem.com/idea-series-ultrasound-capable-3d-printed-central-line-trainer/

## Design Goals & Constraints
Going into the redesign, I set two primary goals:

* **Reduce the size** of the entire trainer system - both the outer head/neck bust and the internal gel piece - to make it more practical for repeated clinical training use.
* **Create hollow, reusable canals** within the gel piece to replicate the jugular vein and carotid artery, without needing to sacrifice tubing on every use.

Achieving these goals meant working around several fabrication constraints:

* **FDM printing wasn't viable for the mold.** Our FDM material of choice, PA-CF, is porous enough that air can pass through the printed layers. Since the trainer needs to be ultrasound-compatible (so trainees can practice using ultrasound guidance, just as they would in a real procedure), any air trapped in or passing through the mold walls would create bubbles that prevent proper ultrasound visualization. This ruled out FDM for the mold itself and pushed me toward resin printing, which produces watertight, air-impermeable parts.
* **Printer limitations added tolerance challenges.** At the time, our Form 2 printer was the only machine in the lab capable of printing in high-temperature resin, but it has noticeably lower speed and dimensional accuracy than the newer Form 4 printers. That meant every mold feature - particularly anything with tight tolerances, like threads - had to be designed with wider tolerances.
* **High-temp resin is brittle.** While necessary for mold durability under repeated use, high-temp resin chips easily under stress. Early testing showed that standard metric threads sheared off when torque was applied, which meant conventional threaded connections weren't a reliable option for any load-bearing or frequently-removed part of the mold.
* **I needed an entirely new mechanism to form the canals.** Since tubing-in-gel was the source of the waste problem, the core design challenge was inventing a way to create hollow canals in the cast gel that didn't rely on a sacrificial part.

## Design Process and Iterations

The solution I converged on was a mold with removable "vein" rods: rigid, precisely-shaped rods that sit inside the mold cavity during casting, physically forming the jugular and carotid canals as negative space, and are then withdrawn after the gel cures - leaving clean, hollow, reusable canals behind instead of embedded tubing.

Getting the rods to insert, seal, and remove reliably took several rounds of iteration:

* **Threading:** Since standard metric threads proved too brittle for repeated use in high-temp resin, I designed my own thread geometry with a round profile and wide pitch. I also added a 0.4 mm face offset, giving enough clearance to account for the Form 2's reduced dimensional accuracy while still creating a secure connection. 
* **Sealing:** I added an O-ring with a chamfered mating face at the rod-mold interface. This let the rod seat securely enough to keep liquid gel from leaking out during casting, without requiring a tight tolerance fit that the printer couldn't reliably produce.
* **Removal:** Each rod was tapered slightly along its length rather than left as a uniform cylinder. The taper let the rod be withdrawn cleanly from the cured gel after casting without tearing the canal, while also helping the surrounding gel form a watertight seal around inserted tubing during actual procedure practice.
* **Size reduction:** Alongside the canal mechanism, I reduced the overall mold volume and the outer head bust volume, cutting down the model's footprint significantly compared to the original full head bust design.

Multiple physical prototypes were printed and cast throughout this process - testing rod removal force, checking for leaks at the threaded interface, and verifying that the cured gel held its shape and canal geometry once the rods were withdrawn.

## Final Result 
The final design is a compact, high-temp resin mold with integrated removable canal rods that casts a puncturable, ultrasound-compatible ballistic gel neck piece, fitting into a significantly downsized head bust. The gel itself replicates the feel and ultrasound appearance of real tissue, letting trainees practice needle insertion and ultrasound-guided localization of the jugular vein and carotid artery. Because the canals are formed by removable rods rather than embedded tubing, the mold can be reused indefinitely - each new training session requires only re-casting the gel, not sourcing and sacrificing a fresh set of tubing. This eliminated the recurring material waste of the original design while also making the overall trainer smaller and easier to store, transport, and prepare for use.

## Mold Components and Result
{% include gallery id="gallery1" %}

## Neck Mold CAD Model
<iframe src="https://vanderbilt1483.autodesk360.com/shares/public/SH28cd1QT2badd0ea72b3e149a25c501f471?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Head Bust and Completed Model
{% include gallery id="gallery2" %}

## Central Line Trainer CAD Model
<iframe src="https://vanderbilt1483.autodesk360.com/shares/public/SH28cd1QT2badd0ea72b19a500eb0df9e7e0?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

