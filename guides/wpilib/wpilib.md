# Prerequisites

Create a new project with the GearsBot example. We'll be analyzing it. A more detailed analysis of command-based programming (which GearsBot is based on) can be found [here](https://docs.wpilib.org/en/stable/docs/software/commandbased/index.html).

# Structure

## `cpp/` vs `include/`

The important parts of the code that'll be edited are in `src/main/cpp/` and `src/main/include/`. Variables, functions, and classes are declared in `include/` while code is written in the respective file in `cpp/`.

## `commands/` vs `subsystems/`

Software links to hardware should be placed in `subsystems/` while commands are in `commands/`. For example, in a smart house, the thermostat and its methods (e.g. getTemperature, setTemperature) are in `subsystems/`. Commands to set temperature to a certain degree, or create a temperature schedule are in `commands/`.

## Command-based Programming

Think of command-based programming like a Discord bot. The bot has multiple commands, like "move back", "throw ball", and "listen to joystick". Commands can be binded to an action, like "throw ball" binded to a joystick button and "move back" to autonomous init. A command can also be set as a default command, which will be run if no other command is active. You can think of it as a bunch of if/elseif/else statements.

```c++
if (button_1.is_pressed()) {
    intake.move_up();
    
} else if (button_2.is_pressed()) {
    intake.move_down();
    
} else {
    default_action();
}
```

# Files

## `Robot.cpp`

There are several methods, following the template of `{period}{schedule}`.

| Period     | Description                      |
|------------|----------------------------------|
| Robot      | Master, whenever the robot is on |
| Disabled   | When robot is not in any mode    |
| Autonomous | When robot is in autonomous mode |
| Teleop     | When robot is in teleop mode     |

| Schedule | Description                                    |
|----------|------------------------------------------------|
| Init     | When the period first starts                   |
| Periodic | Every 20ms (or specified time) during a period |

## `RobotContainer.cpp`

Default commands, autonomous commands, and button binded commands are here.

## `subsystems/Claw.cpp`

Claw is an example subsystem that controls the claw. Claw has custom functions here that commands will call on.

## `commands/OpenClaw.cpp`

OpenClaw is a custom command that calls on the claw subsystem. Commands have several functions that can be overrided.

| Function     | Description                      |
|--------------|----------------------------------|
| initialize() | Similar to the init schedule     |
| execute()    | Similar to the periodic schedule |
| end()        | When the command isFinished()    |
| isFinished() | The condition for the end        |

