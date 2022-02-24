# Simulation Prerequisites

1. Install Visual Studio (**not Visual Studio Code**)
2. During installation, select and install `Desktop Development with C++`

# Creating a Simulation

**The standard setup method is broken on Windows. Use this method:** 

1. Open the Visual Studio Code installed with WPILib
2. Press Ctrl + Shift + P
3. Search and select `WPILib: Create a new project`
4. Choose your options, but make sure Enable Desktop Support is **unchecked, NOT checked, DO NOT CLICK THE BOX**
5. Generate project and wait for the gradle build in the terminal to finish
6. Press Ctrl + Shift + P
7. Search and select `WPILib: Change Desktop Support Enabled Setting`
8. Toggle desktop support on and wait for the gradle build in the terminal to finish

**Standard setup (broken on Windows):**

1. Follow above step 1-4 but check Enable Desktop Support

# Running a Simulation

1. Press Ctrl + Shift + P
2. Search and select `WPILib: Simulate Robot Code`
3. Select `Sim GUI`, and `Sim DriveStart` if that's needed (for exploration purposes, no)
4. Press OK

# Getting Started

1. Create a project with the `Arcade Drive` example, and with simulation support (see above)
2. In `TeleopPeridic()`, add the following:
```c++
m_leftMotor.Set(0.5);
m_rightMotor.Set(0.5);
```
3. In the same method, comment/delete `m_robotDrive.ArcadeDrive(-m_stick.GetY(), m_stick.GetX());`
4. Run the simulation
5. On the top, select NetworkTables > LiveWindow > Ungrouped > DifferentialDrive
6. On the robot status window, select Teleoperated
7. See how the X in the centre of the DifferentialDrive window changes to an arrow
