---
title: Hardware
date: 2021-09-5 00:00:00
weight: 2
---

## Chess Pieces

### Design

Our current prototype design for the chess pieces has a wooden triangle base, 1" ball bearings, two wheels, and two motors. This was chosen to optimize efficiency, while lowering cost, since we have to build 32 chess pieces. The chess pieces themselves are 9.75" x 7.75" x .5", designed for maneuverability on the chess board, so that they can move between other chess pieces and we don't have to worry about moving other pieces out of the way.  
<!--confirm that these are the correct links to the motors-->

<img src="/wiki/active-projects/wizards-chess/images/cad-v1.png" alt="CAD Model of Chess Piece V1" width="600"/>

> Other designs have included an X-drive, 4-wheel drive, or 3-wheel triangle bot, however they were scrapped due to the cost and more complex systems they would have included. 

### Manufacturing

The chess pieces are made from .5" birch plywood and manufactured using the laser cutting and gantry process'. The hole markers are also included in the laser cutting process so that we don't have to remeasure where to drill the holes after every cut and to keep everything uniform.

We will also start manufacturing the motor mounts ourselves to cut down on cost, using 3D printing.

<img src="/wiki/active-projects/wizards-chess/images/laser-cut.png" alt="Laser Cut Lines" width="400"/>
<img src="/wiki/active-projects/wizards-chess/images/motor-mount.jpg" alt="CAD Model of Motor Mount" width="400"/>

## Chess Board

### Design

Each square for the board is 1.5' x 1.5' to accomodate for the chess pieces moving around and between each other. It is then painted black and white accordingly.

> We are actively considering different methods for how to set up the board

### Camera Setup

We are using computer vision and april tags in order to track the pieces as they move around the board. To achieve this a camera setup made of PVC pipe will be placed over the board with several cameras placed in key locations.
