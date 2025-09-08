---
title: "Syringe Pump"
excerpt: "DIY Syringe Pump capable of 1 ul/min flow rate up to 10 ml/min."
header:
  image: assets/img/SyringePump.PNG
  teaser: assets/img/SyringePump.PNG
gallery1:
  - image_path: assets/img/Circuitry.PNG
  - image_path: assets/img/SyringePump.PNG
  - image_path: assets/img/Wiring.png
gallery2:
  - image_path: assets/img/Enclosure.png
  - image_path: assets/img/enclosure-side-drawing.png
  - image_path: assets/img/enclosure-top-drawing.png
  - image_path: assets/img/motor-mount-drawing.png
  - image_path: assets/img/carriage-drawing.png
  - image_path: assets/img/syringe-support-drawing.png
   
---

# Features

* **Precision Drive:** Powered by a stepper motor coupled to a lead screw, the pump delivers highly accurate and repeatable motion. Flow rate is fully programmable in the Arduino code with a single variable.
* **Syringe Flexibility:** Compatible with 10–20 mL syringes, which can be loaded and secured without tools. Both ends of the syringe are supported to eliminate sagging during operation, ensuring consistent flow.
* **Simple Controls:** Intuitive user interface with a latching start/pause button and a built-in limit switch to automatically stop when the syringe is empty.
* **LED Status Indicator:** Clear visual feedback provided by the LED light: 🟢 green when running, 🟡 yellow when paused, and 🔴 red when the syringe is empty.
* **Clean & Compact Design:** Electronics are combined into a single protected enclosure that shields the power supply, Arduino, and breadboard from users and liquid exposure. Soldered and heat-shrinked connections keep wiring tidy and secure.
* **User-Friendly Extras:** Two momentary buttons allow manual forward/backward motor control for quick syringe setup, and a potentiometer enables real-time flow rate adjustments.


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a408db1211465ff366?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
{% include gallery id="gallery1" %}

## 3D-Printed Components

| Component             | Material |
|-----------------------|----------|
| Enclosure Bottom      | PLA      |
| Enclosure Side Panel  | PLA      |
| Enclosure Top         | PLA      |
| Motor Mounting Piece  | ABS      |
| End Support           | ABS      |
| Carriage              | ABS      |
| Syringe Support       | ABS      |


## Off-the-Shelf Components

| Component                                   | Specification / Model                                  | Quantity |
|---------------------------------------------|--------------------------------------------------------|----------|
| Lead Screw                                  | 250 mm, 2 mm pitch, 2 mm lead                          | 1        |
| Lead Screw                                  | 250 mm, 2 mm pitch, 8 mm lead                          | 1        |
| Flexible Coupling                           | 1/4" x 8 mm                                            | 1        |
| Linear Rod                                  | 200 mm, 8 mm diameter                                  | 2        |
| Linear Bearing                              | LM8UU, for 8 mm rod                                    | 2        |
| Aluminum Extrusion                          | 2040, 1 ft length                                      | 1        |
| Stepper Motor                               | NEMA 17                                                | 1        |
| Power Supply                                | MEAN WELL RQ-65D AC-DC Quad Output (5V, 12V, 24V, 12V, 4A) | 1        |
| Arduino Board                               | Arduino Uno (GrabCAD model)                            | 1        |
| Stepper Driver                              | A4988                                                  | 1        |
| Breadboard                                  | Small                                                  | 1        |
| Push Button (Latching)                      | Panel-mount, On/Off                                    | 1        |
| Push Button (Momentary, bonus only)         | Panel-mount                                            | 1        |
| Limit Switch                                | Standard                                               | 1        |
| LED                                         | RGB, common cathode                                    | 1        |

{% include gallery id="gallery2" %}





