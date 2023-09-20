---
title: Wizard's Chess
date: 2021-07-30
weight: 4
no_list: true
description: >
    Building a giant, automated chess board
---

## Goal

Our goal for this project is to be able to create a fully autonomous, life sized chess game that people will be able to play using only voice commands. This project was inspired by the Wizard's Chess game in Harry Potter and the Philosopher's Stone. We will be exploring different hardware and software concepts, including engineering design, CAD, manufacturing, computer vision, and trajectory planning.

## Subsystems

### Hardware
We are currently working on developing all 32 pieces for the game, as well as manufacturing the chess board ourselves. Navigate to our [hardware docs]({% link wiki/wizards-chess/hardware.md %}) to understand where we are at in terms of our hardware progress.

#### CAD
The CAD team is utilizing Fusion 360 to create a model of the basic chess piece. They are also our go-to team for laser cutting, 3D printing, CNCing, and general manufacturing, especially when it comes to needing certain files.

### Software
We will be working on vision using apriltags to determine the positioning of each of the pieces on the board on an x,y coordinate plane and voice inputs to direct the pieces where to go.  This will all be controlled by the overarching Raspberry Pi 4 controller, intakes voice commands, determines valid moves, and calculates the correct trajectory for each of the pieces. Navigate to our [software docs]({% link wiki/wizards-chess/software.md %}) to get a deeper dive into these concepts.

#### Computer Vision
This team is tasked with figuring out how to capture the position of all pieces on the board at all times. The current design is to use an overhead camera that will encompass the whole board, and then use Apriltags on each robot and 4 corners. With this information, we will be able to digitally map them on an xy-coordinate plane and perform the trajectory and pathing calculations correctly in order to move the correct chess pieces to the correct spots.

#### Voice Recognition
This team is tasked with implementing full voice recognition capabilities for the chess game. They are looking into different voice recognition libraries that will be the best to implement in order to assist the creation of the software needed. The voice recognition software will take different commands (ie: Knight to e4) and use the trajectory planner to convert them to a point on the plane for the piece to move to.

#### Controls
This team is tasked with determining how to control the robots using wifi to play the chess game. The pieces will have to move according to the commands given from voice recognition and be able to adjust their path should they veer off course. 

## What have we been up to?

### Spring 2023 

- Made more robots!
  - We now have 8 fully functional robots
  
<img src="images/WC-prototype1.jpg" alt="Chess Piece Prototype" width="400"/>

- Started designing camera set up for computer vision

{{< drive-player "18uXqdxGblfsNUdoEI2qEVPu5-sYCvQ7a/preview" >}}

- Wrote code to allow robots to communicate with computer over wifi and send commands
- Scanned april tags to disguish between pieces and orientation

## Plans for the Future

We are planning on creating low-poly structures for each of the chess pieces and combining them with LED indicators to distinguish between the different pieces. We will also be looking into creating custom PCBs for each of the robots.
