---
title: "SkyScan"
author: "Wrexik"
description: "An autopilot 4'' FPV drone with INAV and OpenIPC used for photogrametry!"
created_at: "2025-05-21"
---

# 05-21: Initial Repository Creation & Ideas
``Aprox. 2,5 hours of research``

Created a new repository for the SkyScan project.
I've watched videos on drone building and the INAV firmware.
- Looked into ELRS and OpenIPC for long-range control and video streaming.

 Wrote down the following features I would like to acomplish:
  - Under 250g due to regulations
  - 4" frame
  - Digital FPV with OpenIPC
  - 4S battery
  - GPS and Mission planning with INAV
- Looked into compatibility of OpenIPC and ELRS frequencies. Both are 2.4GHz. So i will need to use a 900MHz ELRS module. To make sure that the 2.4GHz and 900MHz modules are not **interfering with each other**.
- Looked up options for the OpenIPC system. Decided to go with **Wyvern Link (Alpha) OpenIPC - 100mW VTX** for its price and good camera.

Aliexpress will be the shop I will be sourcing from, cheap shipping and a huuuge selection of parts. I have only good experience with Aliexpress. So there isn't another option.

Okay, few hours later and I have actually a better option for the camera. I will be using the **Eachine Sphere Link 5.8GHz WIFI Digital HD**. Since the Wyvern Link does not support onboard recording. This will be much better option. And I will be able to use the **5.8GHz** frequency for the video and 2.4ghz for the ELRS.

> this is the Eachine Sphere VTX
![[Video TX.jpg]]

- This was about 2,5 hours of research. I will be continuing to look into the components and their compatibility.
# 05-21: Frame, FC, Motors
I prioritized selecting the camera first because thats the main part of the drone for the actuall 3D scanning.

I've continued to look up parts and I think I have a quite good combination now. I'm especially happy with the frame. It's built so the props dont show in the camera feed. **Clear video is important!** 
### As of now, I have selected the following components:

| Component                   | Details / Notes                                                                               |
| --------------------------- | --------------------------------------------------------------------------------------------- |
| **Frame**                   | **JMT LR4 169mm (4")** — supports 20x20 / 25.5x25.5mm stacks                                  |
| **Flight Controller + ESC** | **SpeedyBee F405 AIO 40A** — powerful, 25.5x25.5mm mount (fits with adapter or printed plate) |
| **Motors**                  | **T-Motor P1604 3800KV** — perfect for 4S & 4" props; great efficiency for cruising           |
| **Camera/VTX**              | **Eachine Sphere Link** — 1080p onboard DVR, MAVLink, 800mW digital FPV                       |
| **Receiver**                | **Radiomaster XR1 Nano ELRS** 2.4GHz/900MHz dual-band — fully INAV + ELRS compatible          |
>  The frame I've chosen to go with
![[Frame.jpg]]

next steps:
- Look into the GPS recomended by the frame manufacturer. Since it already has a GPS mount.
- Learn more about props and their compatibility with the motors.
- Finish with battery selection. **And establish a weight budget.**

My plan for the custom parts are legs that I will model and 3D print. I will also be using a 3D printed mount for the camera. As of custom hardware, the FC has a I2C port, I could use that for a LIDAR or RGB.

Thats all for now. Will be back soon!

# 05-22: Component Selection & Weight Budget
`2 hours to school well spent :P`

Hey again, today I started working right after I got into my train. I've decided on gps module that will be needed for the drone to have a good possition hold while taking pictures. 
The GPS should also have an magnetometer. For the drone to know direction. Which the **Beitian BN-880 BN880** has.

Iast night I've watched a few video's and all of the featured drones had a buzzer. So I figured I might also add one, the FC supports it.

| Component  | Details / Notes                                                                                                               |
| ---------- | ----------------------------------------------------------------------------------------------------------------------------- |
| **GPS**    | **Beitian BN-880 BN880 Flight Controller GPS** - Fast and accurate, has magnetometer                                          |
| **Buzzer** | **Pixhawk PX4 Buzzer** - really compact                                                                                       |
| **Props**  | **Gemfan 4023 1.5mm 2mm 4inch 3 blade** - Good looking and in the right size. They should be made for the brand of our motors |
Now I'm looking into props. They should have 1.5mm hole and 3 blades. 4 inch size of course. 

From what i understand the **4023** are suitable.
I've chosen a **pack of 16**. Since they are quite fragile. 

I really like this looking up parts and matching them with each other. Its like building computers but it FLIES!

With the props added it looks quite complete, just checking few thing's with the seller of the drone frame so I could be sure with the dimensions. I CANT WAIT!

I will be sourcing my own batteries & controller. The software part is also what im looking forward, I found some that I could modify for my 3D scanning implementation!

I will have my friend run over the parts and check some of the fitment. The VTX will have to have a custom 3D printed adapter. Because its 0.5mm off. Thats no problem, I will practice my patience and CAD skills. 

Also interesting thing I found was this RX module while I was looking up options with the interfering frequencies was the current **Radiomaster XR1 Nano ELRS** it is dual band. So it supports both 2.4GHz and 900MHz. So I could upgrade for longer range down the road!

![[RX.jpg]]

Hey im back, 2 classes after, I've found this cute pair of lollipop antennas, they will be great for the VTX. Since the drone will be operated by remotely on a monitor I would really like a good video feed. Might implement comuter vision for object detection.

![[Lollipop antennas.jpg]]

# 05-23: Final costs & pitch

`took more or less about an 30 minutes`

| Parts       | Link                              |  Costs  + Shipping  |
| ----------- | --------------------------------- | :-----------------: |
| Frame       | https://a.aliexpress.com/_EvwVZDU | 730 CZK - 33,15 USD |
| VTX         | https://a.aliexpress.com/_EHbSKhC | 2350 CZK - 107 USD  |
| Motors      | https://a.aliexpress.com/_EINYVGa |  1142 CZK - 52 USD  |
| VTX Antenna | https://a.aliexpress.com/_Ev1Kqw6 |  300 CZK - 14 USD   |
| FC AIO      | https://a.aliexpress.com/_Ez89AS2 |  1330 CZK - 61 USD  |
| Buzzer      | https://a.aliexpress.com/_EHUrHM6 |   45 CZK - 2 USD    |
| Props       | https://a.aliexpress.com/_EzHnXNG |   130 CZK - 6 USD   |
| GPS         | https://a.aliexpress.com/_ExEMGLG |  600 CZK - 27 USD   |
| RX          | https://a.aliexpress.com/_ExRInKe |  335 CZK - 15 USD   |

## Pitch

Hey @alexren!
My name is Kryštof and study IT in 🇨🇿.

I would like to pitch my idea of my little project. Month ago I was introduced to the amazing world of 3D scanning. I usually go around an object and take a ton of photos with my phone. But only where my hand can reach. 

This beach scan is a good example:
https://splatter.app/s/c07-ax0

I've attended 3DISE conference in Prague, met a lot of smart people. And I was fascinated by one presentation. Scanning the whole Alcatraz. It would be possible without drones. Seeing the objects from the top would enable me to scan abandoned buildings and continue exploring the topic of photogrammetry and 3D gaussian splatting.

DJI has it's own enterprise solution for 3d scanning, so why wouldn't we make it too and open source. Autonomous digitizing of buildings and sites.

**Examples of recent previous work:**
- SMD alarm clock, with 2 switches and buzzer to configure and wake you up. ![[Clock.jpg]]
**What would be the build process:**
1. Gather all the hardware needed.
2. 3D model new mount for the camera and VTX adapter.
3. 3D print the rest of the frame with modification to fit the antennas.
4. Practice soldering & planing the steps.
5. Configure, Build, Code and Fly!


**BOM:**
- Frame - 730 CZK / 33.15 USD
- VTX - 2350 CZK / 107 USD
- Motors - 1142 CZK / 52 USD
- VTX Antenna - 300 CZK / 14 USD
- FC AIO - 1330 CZK / 61 USD
- Buzzer - 45 CZK / 2 USD
- Props - 130 CZK / 6 USD
- GPS - 600 CZK / 27 USD
- RX - 335 CZK / 15 USD

**Why I know I can do this:**
I wanted to build my own drone for a while. It is a fascinating hobby for me, and I want to get into it. And where else to start, just build one. I have pretty good knowledge in IT software side, but this could open my heart to pcb designing and hardware. 

**Why this deserves 10 points?**
- It has quite a lot of new things for me to learn and explore.
- I think it is a unique idea, that could open this world for others like it did for me.
- I might not be making something super complex but I will be building something that was on my mind for a while. Super motivated about this.

Thanks for reading in, 💕 Wrexik.