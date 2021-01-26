# ![logo](/MARR_logo.png)Microsoft Applied Robotics Research Library

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  

This library contains repositories containing software applications, data sets, and hardware reference designs to support research and education in the fields of service-robotics. Our team invites you to join us in research and engineering efforts that consider how robots can assist and augment the capabilities of human beings.

Current projects focus on the field of **Human-Robot-Interaction** with the goal of providing service robots the means to effectively communicate with humans. In the future we plan to offer new repositories exploring the fields of robot **Navigation** and object **Manipulation**.

## Human-Robot Interaction (HRI)
The field of HRI concerns solutions for robot speech, expressions, gestures, and information access to provide natural methods for robot command and control.

### Labanotation Suite
The Labanotation Suite is a collection of repositories comprising a system that can be used to give service robots the ability to move in natural and meaningful ways. It includes software tools, source code, sample data, hardware design kits and simulation software that supports experimentation with the concepts presented in the paper **[Describing Upper-Body Motions Based on Labanotation for Learning-from-Observation Robots](https://link.springer.com/article/10.1007%2Fs11263-018-1123-1) (International Journal of Computer Vision, December 2018)**.

#### Gesture Authoring Tools
https://github.com/microsoft/LabanotationSuite

The Gesture Authoring Tools repository provides an upper-torso human-gesture capture and editing solution. The system consists of compiled gesture capture applications using the Microsoft Kinect sensor device and a Windows 10 PC. Editing tools constructed in Python provide gesture trimming and movement analysis options with output in graphical Labanotation scores as well as movement data expressed in Labanotation and implemented in a JSON data format. 

#### gestureBot Design Kit
https://github.com/davidbaumert/gestureBotDesignKit

With a Windows 10 PC, and optionally a 3D-printer and about $350(USD) in electronic servos and parts, the gestureBot Design Kit repository contains all the information needed to build both a virtual and physical desktop companion robot. It includes browser-based simulation and control software based on the Robotis XL series of servo motors. To construct a physical robot, it provides models for 3D-printable body-parts, a parts-list for electronic components, and step-by-step assembly instructions. No soldering is required, but some manual skill is needed to mate small electronic connectors, as well as manipulate small plastic rivets and miniature metal screws to assemble the body components.

#### Gesture Library
https://github.com/davidbaumert/GestureLibrary

The Gesture Library is a data-set comprised of upper-torso gestures expressed in Labanotation and implemented in a JSON format.

#### Gesture Service
https://github.com/davidbaumert/GestureService

The Gesture Service project is a software module constructed with Python and Google's neural network [word2vec](https://code.google.com/archive/p/word2vec/#!) that takes a text phrase as input and returns a corresponding gesture.

#### MSRAbot AirSim Design Kit
https://github.com/davidbaumert/MSRAbot_DesignKit

With a gamer-class Windows 10 PC, and optionally a 3D-printer and $800(USD) in electronic servos and parts, the MSRAbot AirSim Design Kit repository contains all the information needed to build both a virtual and physical mobile companion robot. It includes browser-based simulation and control software based on the [Futaba RS](https://futabausa.com/product/rs303mr/) series of servo motors. To construct a physical robot, it provides models for 3D-printable body-parts, a parts-list for electronic components, and step-by-step assembly instructions. Intermediate electronic assembly and soldering skills are required to build the physical robot. To place a virtual model of the robot in a 3D simulation environment, an implementation hosted in [**Microsoft AirSim**](https://github.com/microsoft/AirSim) is provided to support AI model training and robotics research projects.


***(the following projects and descriptions comprising our project roadmap ARE NOT included in public repositories)***            


#### Full-Humanoid Gesture and Dance Capture

#### Full-Humanoid Gesture and Dance Performance

## Navigation
The field of robot navigation concerns solutions such as simultaneous-location-and-mapping (SLAM), path planning, and map management.

### Hololens Indoor Navigation
This project shows how a Hololens device can be placed on the head of [Softbank Robotics' Pepper robot](https://us.softbankrobotics.com/pepper) and provide a self-calibrating indoor navigation solution within a single room.

### Azure Kinect Indoor Navigation
This project shows how an Azure Kinect device can be placed on a mobile delivery robot and provide a self-calibrating indoor navigation solution within a large building.

## Manipulation
Common in industrial-robotics where actions are manually programmed and repeated, the field of robotic object manipulation is much more challenging in service-robotics scenarios. Our projects explore solutions where HRI and Navigation technologies can be leveraged to allow robots to learn from humans to perform manipulation tasks safely and effectively in dynamic residential, workplace, and public environments. 

### Human-trained Object Manipulation
This project shows how a human who is expert in a given task can use HRI solutions and AI-based task-planning to teach a service robot to reliably perform the same task within a dynamic environment.
