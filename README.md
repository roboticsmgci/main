# Table of Contents

1. [Tasks](https://github.com/roboticsmgci/main#tasks)
    1. [Robot](https://github.com/roboticsmgci/main#robot)
    2. [Vision](https://github.com/roboticsmgci/main#vision)
    3. [General](https://github.com/roboticsmgci/main#vision)
2. [FAQ](https://github.com/roboticsmgci/main#faq)

---

# Tasks

## Robot

1. Work with simulation
    1. Start with [this](https://github.com/roboticsmgci/main/blob/main/guides/wpilib/simulation.md)
    2. Experiment with different motor values
    3. Get Field2D working by reading the guides and documentation
2. Run the motor directly through your laptop with the [SparkMax API](https://docs.revrobotics.com/sparkmax/software-resources/spark-max-api-information#c-api)

**Notes**
- The WPILib guide does say you can use your keyboard as a controller, but the example codes are set up with joystick as a controller
    - Ignore that part, or plug in the joystick (in-person) to test
- [WPILib C++ API](https://first.wpi.edu/wpilib/allwpilib/docs/release/cpp/index.html) has some very useful information, include what to `#include`

## Vision

1. Work on [OpenCV practice exercises](https://github.com/roboticsmgci/main/blob/main/vision/practice-exercises.md)
2. If you have a Raspberry Pi, take a camera and start working through [this tutorial](https://docs.wpilib.org/en/stable/docs/software/vision-processing/wpilibpi/index.html)
3. If you don't, take a camera (if there are remaining), [install Python and the OpenCV library](https://github.com/roboticsmgci/main/blob/main/guides/python.md), and experiment with object detection, edge detection, and other features. 
4. Try to attach a camera to the roborio and display the feed on the driver station software — you will need to supply the camera with power, so work with building for this.

## General

1. Help with building

---

# FAQ

## How did you format this?
Markdown. Here's a guide: https://www.markdownguide.org/cheat-sheet/

## Should I make pull requests to edit?
Just edit a file directly, through GitHub's built-in editor or whatever floats your boat. There's no need to write commit messages either, use the default.

## Why does it say the language is Shell?
The green icon of Shell pops out in the sea of dark mode and makes this repo easier to find.
