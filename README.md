# HW4: AR Tracking and 3D Reconstruction with OpenCV

For this homework you will be implementing pose estimation of a known image using OpenCV. You will then adapt this pose estimation algorithm to compute a sparse point cloud representation of a scene. This homework is intended to give you a basic introduction to computer vision as it relates to augmented reality. This includes concepts such as camera calibration, feature matching, perspective projection, and 3d point cloud estimation. 

In this homework you will be guided through most of the steps to implement AR pose estimation of a known image, but you will be asked to implement one basic function based on the concepts we introduced in class. You will then use what you have learned to develop a system for sparse point cloud reconstruction of a scene using your mobile device. These steps represent a simplified set of functions that form the basis of modern AR tracking. 


 

## Logistics

Use the repository created when you accept the assignment on GitHub classrooms (this repo). The course staff will look at this repo to evaluate your code for this assignment, so please make sure you submit your code into this repository when you turn in your assignment.

### Academic honesty
Please do not post code to a public GitHub repository, even after the class is finished, since these HWs will be reused both  in the future.

This HW is to be completed individually. You are welcome to discuss the various parts of the HWs with your classmates, but you must implement the HWs yourself -- you should never look at anyone else's code.

## Deliverables:

### 1. Video

You will make a 2 minute video showing off your implementation. You should verbally describe, at a very high level, the concepts used to implement the image pose tracking and 3d reconstruction. You must also include captions corresponding to the audio.

### 2. Code
You will also need to push your project folder to your repo (this repo). Add the following github IDs so that we can access these:

## Before You Start:
For this homework you will need Python and OpenCV. 

### To install python (if you do not have it already installed)

OS X and linux machines, python comes pre-installed. 

In case you do not have it installed, we recommend installing the Anaconda environment.

Download _Anaconda_ with _Python 3.11_ from here - https://www.anaconda.com/products/individual and install it with default options.

**If your version of the installer has different version numbers than these screenshots, that is OK.**

![inst1.png](/Instructions/inst1.PNG)
![inst2.png](/Instructions/inst2.PNG)
![inst3.png](/Instructions/inst3.PNG)
![inst4.png](/Instructions/inst4.PNG)
![inst5.png](/Instructions/inst5.PNG)

### To install opencv within Anaconda

Choose _Anaconda prompt_ from the start menu, and "Run as Administrator".

![inst6.png](/Instructions/inst6.PNG)

First run this command to update anaconda. For some of these commands, you may be asked to confirm the command with y or n

```python
conda update -n base -c defaults conda
```

In the Anaconda prompt, we will first create a new Python environment for HW3. This will use Python version 3.11
```python
conda create -n hw3env python=3.11
```

Next we will activate this environment. Note you need to run your HW code in this environment, since this is the one in which we wilol be installing openCV
```python
conda activate hw3env
```

Once activated, we will install OpenCV 4.8.1 in it
```python
pip install opencv-contrib-python==4.8.1.78
```

You can choose to run your program in any of the python IDEs in _Anaconda_ such as _Spyder_, but make sure to select the _hw3Env_ before you launch and install the IDE.

![inst7.png](/Instructions/inst7.PNG)

## Install OpenCV without Anaconda
To install OpenCV outside of Anaconda, In command prompt/ terminal run:

```python
pip install opencv-contrib-python==4.8.1.78
```
(you may need to add sudo for unix systems). 

Note: This document was written using OpenCV 4.8.1. Some changes may be required for alternate versions of OpenCV.

## Instructions

Instructions for setting up the starter code are available at the google docs file at https://docs.google.com/document/d/1g3e9IZeJz_PfN5nqvuF8QO-nIbhromvIVWBmqXaFmF0


