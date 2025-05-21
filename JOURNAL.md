---
title: "SkyScan"
author: "Wrexik"
description: "An autopilot 4'' FPV drone with INAV and OpenIPC used for photogrametry!"
created_at: "2025-05-21"
---

# 05-21: Initial Repository Creation & Ideas
- Created a new repository for the SkyScan project.
- Watched videos on drone building and the INAV firmware.
- Looked into ELRS and OpenIPC for long-range control and video streaming.
 Wrote down the following features I would like to acomplish:
  - Under 250g due to regulations
  - 4" frame
  - Digital FPV with OpenIPC
  - 4S battery
  - GPS and Mission planning with INAV
- Looked into compatibility of OpenIPC and ELRS frequencies. Both are 2.4GHz. So i will need to use a 900MHz ELRS module. To make sure that the 2.4GHz and 900MHz modules are not **interfering with each other**.
- Looked up options for the OpenIPC system. Decided to go with **Wyvern Link (Alpha) OpenIPC - 100mW VTX** for its price and good camera.

Okay, two hours later and I have actually a better option for the camera. I will be using the **Eachine Sphere Link 5.8GHz WIFI Digital HD**. Since the Wyvern Link does not support onboard recording. This will be much better option. And I will be able to use the **5.8GHz** frequency for the video and 2.4ghz for the ELRS.

- This was about 2 hours of research. I will be continuing to look into the components and their compatibility.
### As of now, I have selected the following components:

| Component                      | Details / Notes |
|-------------------------------|------------------|
| **Frame**                     | **JMT LR4 169mm (4")** — supports 20x20 / 25.5x25.5mm stacks |
| **Flight Controller + ESC**  | **SpeedyBee F405 AIO 40A** — powerful, 25.5x25.5mm mount (fits with adapter or printed plate) |
| **Motors**                    | **T-Motor P1604 3800KV** — perfect for 4S & 4" props; great efficiency for cruising |
| **Camera/VTX**                | **Eachine Sphere Link** — 1080p onboard DVR, MAVLink, 800mW digital FPV |
| **Receiver**                  | **Radiomaster XR1 Nano ELRS** 2.4GHz/900MHz dual-band — fully INAV + ELRS compatible |

next steps:
- Look into the GPS recomended by the frame manufacturer. Since it already has a GPS mount.
- Learn more about props and their compatibility with the motors.
- Finish with battery selection. **And establish a weight budget.**

My plan for the custom parts are legs that I will model and 3D print. I will also be using a 3D printed mount for the camera. As of custom hardware, the FC has a I2C port, I could use that for a LIDAR or RGB.

Thats all for now. Will be back soon!

# xx-xx: Component Selection & Weight Budget
