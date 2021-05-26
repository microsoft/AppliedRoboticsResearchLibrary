## **![logo](./MARR_logo.png) Microsoft Applied Robotics Research Library**

### Open Source Samples for Service Robotics
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  

This library is a collection of GitHub repositories containing software applications, data sets, and hardware reference designs to support research and education in the fields of service-robotics. Our team invites you to join us in research and engineering efforts that advance how robots can assist and augment the capabilities of human beings.

Current projects focus on the field of **Human-Robot-Interaction** with the goal of providing service robots the means to effectively communicate with humans. In the future we plan to offer new repositories exploring the fields of robot **Navigation** and object **Manipulation**.

## Human-Robot Interaction (HRI)
The field of HRI includes robot speech, expressions, gestures, and information access to provide natural user interface methods for robot applications.

### [Labanotation Suite](https://github.com/microsoft/LabanotationSuite)
The Labanotation Suite is a collection of applications comprising a system that can be used to give service robots the ability to move in natural and meaningful ways. It includes software tools, source code, sample data, and hardware simulation software that supports experimentation with the concepts presented in the paper **[Describing Upper-Body Motions Based on Labanotation for Learning-from-Observation Robots](https://link.springer.com/article/10.1007%2Fs11263-018-1123-1) (International Journal of Computer Vision, December 2018)**. The system consists of compiled gesture capture applications using the Microsoft Kinect sensor device and a Windows 10 PC. Editing tools constructed in Python provide gesture trimming and movement analysis options to identify key points of movment. Output is graphical Labanotation scores as well as movement data expressed in Labanotation and stored in JSON data format. 

#### **[KinectReader: ](https://github.com/microsoft/LabanotationSuite/tree/master/GestureAuthoringTools/KinectReader) Human Gesture Capture Tool**

A compiled Windows application that connects to a Kinect sensor device and provides a user interface for capturing and storing gestures performed by human subjects. It's primary output data is human stick-figure joint positions in a .csv format, but can also capture corresponding RGB video and audio at the same time.

#### **[KinectCaptureEditor: ](https://github.com/microsoft/LabanotationSuite/tree/master/GestureAuthoringTools/KinectCaptureEditor) Human Gesture Trimming Tool**
A compiled Windows application that loads human joint position .csv files produced by the KinectReader or other tools, as well as optional corresponding video and audio files. It provides a timeline-based method to trim audio and video joint movement sequences into representative human gestures.

#### **[LabanEditor: ](https://github.com/microsoft/LabanotationSuite/tree/master/GestureAuthoringTools/LabanEditor)  Gesture Analysis and Labanotation Generator**
A Python application that loads a Kinect joint .csv file representing a human gesture, provides algorithmic options for automatically extracting keyframes from the gesture that correspond Labanotation data, and provides a graphical user interface for selection and modification of the extracted keyframes. Additionally, it saves the resulting gesture data in a JSON file format suitable for controlling robots running a gesture interpretation driver, as well as .png graphic file renderings of the charts and diagrams used in the interface.

#### **[MSRAbotSimulation: ](https://github.com/microsoft/LabanotationSuite/tree/master/MSRAbotSimulation)  Gesture Performance with Simulated Robot**
This Python and browser-based simulation software uses javascript and html code to implement an animated 3D model of the robot and a user interface for selecting and rendering gestures described in the JSON format. A temporary local HTTP server invoked with python or an existing server can be used to host the software and the simulation is run within a modern web browser. The user can choose from a collection of sample gestures, or select a new gesture captured and created using this project's Gesture Authoring Tools.

### [gestureBot Design Kit](https://github.com/microsoft/gestureBotDesignKit)

With a Windows 10 PC, and optionally a 3D-printer and about $350(USD) in electronic servos and parts, the gestureBot Design Kit repository contains all the information needed to build both a virtual and physical desktop companion robot. It includes browser-based simulation and control software based on the [Robotis XL](https://www.robotis.us/dynamixel-xl-320/) series of servo motors. To construct a physical robot, it provides models for 3D-printable body-parts, a parts-list for electronic components, and step-by-step assembly instructions. No soldering is required, but some manual skill is needed to mate small electronic connectors, as well as manipulate small plastic rivets and miniature metal screws to assemble the body components.

#### **[Gesture Library: ](https://github.com/microsoft/gestureBotDesignKit/tree/main/src/Labanotation) Example Set of Upper-Torso Gestures**

The Gesture Library is a data-set of upper-torso gesture-concept pairs expressed in Labanotation format and stored as .json files. The data is directly accessed by the Gesture Engine. The library includes a complete listing of the sample database including a video clip of each gesture performed by the gestureBot.

#### **[Gesture Service:  ](https://github.com/microsoft/gestureBotDesignKit/tree/main/src/Samples/gestureService_w2v) Example Gesture Service Engine**

The Gesture Service project is a software module constructed with Python and Google's neural network [word2vec](https://code.google.com/archive/p/word2vec/#!) that takes a text phrase as input and returns a corresponding gesture.

## Navigation
The field of robot navigation includes systems and methods such as simultaneous-location-and-mapping (SLAM), path planning, and map management.

#### **[HololensNavigation:  ](https://github.com/microsoft/HololensNavigation)Self-calibrating Indoor Navigation**
This project shows how a [Hololens](https://www.microsoft.com/en-us/hololens) device can be placed on the head of [Pepper robot](https://us.softbankrobotics.com/pepper) and provide a self-calibrating indoor navigation solution within a single room.

## Manipulation
In industrial applications, robotic object manipulation is common where actions are manually programmed and repeated behind safety barriers. In service-robotics scenarios, dynamic environments and safety considerations make the entire field much more challenging. Our projects explore solutions where HRI and Navigation technologies can be leveraged to allow robots to learn from humans to perform manipulation tasks safely and effectively in residential, workplace, and public environments. 

While we are working towards an open-source object-manipulation sample for service-robotics next year, our team-mates at Microsoft Bonsai are forging ahead with Autonomous Systems for industrial applications.  Take a look at [Project Moab](https://microsoft.github.io/moab/).

