# Prerequisites

1. Install [Visual Studio](https://visualstudio.microsoft.com/downloads/) (**not Visual Studio Code**)
2. During installation, select and install `Desktop Development with C++`

# Creating a Simulation

**Checking *Enable Desktop Support* does not work in Windows 10 WPILib 2022. Even if you use another OS, it's recommended to use this as it's more consistent.**

1. Open the Visual Studio Code installed with WPILib
2. Press Ctrl + Shift + P
3. Search and select `WPILib: Create a new project`
4. Choose your options, but make sure Enable Desktop Support is **unchecked, NOT checked, DO NOT CLICK THE BOX**
5. Generate project and wait for the gradle build in the terminal to finish
6. Press Ctrl + Shift + P
7. Search and select `WPILib: Change Desktop Support Enabled Setting`
8. Toggle desktop support on and wait for the gradle build in the terminal to finish

# Running a Simulation

1. Press Ctrl + Shift + P
2. Search and select `WPILib: Simulate Robot Code`
3. Select `Sim GUI`, and `Sim DriveStart` if that's needed
4. Press OK
