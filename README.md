# MECA482_BallNPlate_Team2
### MECA 482 Control System Engineering Project
----------------------------------------------------------------------------------

Ball N Plate Control System Design
<p align = "center">
  Project Members:
  Travis Bybee,
  Chris Leach,
  Matt Firpo,
  Alberto Rosales
  </p>
  
  <center>
   <h4> California State University Chico</h4>
   <h4> College of Mechanical and Mechatronic Engineering and Advance Manufacturing</h4> 
   <h4> MECA 482 Control System Engineering</h4> 
   <h4> Ball N Plate</h4> 
</center>

#### Table of Contents
- [1. Introduction](#1-Introduction)
- [2. System Requirements](#2-System-Requirements)
- [3. Mathematical Model](#3-Mathematical-Model) 
- [4. Simulink](#4-Simulink) 
- [5. Coppelia Simulation](#5-Coppelia-Simulation)
- [6. Appendix](#6-Appendix)
- [7. References](#7-References)

## 1. Introduction 
The purpose of this project is to incorporate everything we have learned from this past semester 
in order to create a real life example of a working control system.
The system consists of a plate which can be tilted by two servo motors or electric motors
in two different angular orientations together with a ball rolling around on top of the plate.
The goal was to design a controls system that allows the user to put a ball anywhere on the plate and have the servo motors 
position the ball in the center of the plate.

## 2. System Requirements

The System Requirements of this project....

## 3. Mathematical Model

Mathematical model:


Insert Photos



This is the block diagram corresponding to one axis of our 2 degrees of freedom ball balancer system. This specific diagram has two loops, the inner loop on the right represents the model of the servo Ps(s), and the ball balancer model. The outer loop on the left is representing the position controller S. The position controller is to be implemented in Simulink and the servo controls and ball balancer models are to be implemented into coppeliasim.

Insert Equations



The equations above represent our block diagram respectively for one axis of the 2 degree of freedom ball balancer. It follows the format of a standard second-order system therefore we can go ahead and solve for our proportional gain KP and derivative gain KD using our system parameters of percent overshoot, and settling time. For our system, we’re using a 10% overshoot, with a 4% settling time of 5 seconds, and a Steady-State error of  7.5mm.

In the overall system, the same transfer function will be implemented for the second axis of the 2 degree of freedom ball balancer system. This is a workaround to create a MIMO system by combining multiple SISO systems. One of the diagrams will be for the X-axis, and the other will be for the Y-axis. Therefore the mathematical model for the entire system will be encompassed by both of these equations. 


	The mathematics for our project can be described by the inherent mathematical equation relating to a PID controller. This equation is seen below. 
INSERT PHOTO

Where KP is the proportional gain, Kiis the integral gain, and K is the derivative gain. This specific system is replicated by a PD controller, meaning Ki is equal to zero. 


## 4. Simulink

The Simulink Model created ....

## 5. Coppelia Simulation

The Coppelia Simulation which proves that our algorithms facilitate the designated system requirements...

## 6. Appendix 

A1:

A2:

## 7. References
[1] Nise, Norman S. Control Systems Engineering. Hoboken, NJ: Wiley, 2015. 


