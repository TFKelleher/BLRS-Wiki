---
description: >-
  Vex drivetrains are assemblies, generally made of wheels, used to traverse the
  VRC field. Each drivetrain has its own set of advantages and disadvantages.
---

# Types of Motion

When designing a drivetrain, there are multiple forms of drive train that can be considered.
The first is a static drivetrain. These are the most common and easiest to build, program, and maintain.
The second is a holonomic drivetrain. This category is defined as having the ability to move in a direction that is not directly front or back of a robot. Holonomic Drivetrains take many forms, and each has its own use cases.

## Static Drivetrains

A Static Drivetrain only has one implimentation, most commonly known as a "Tank Drive", pictured here.

![Tank Drive](https://user-images.githubusercontent.com/65926085/83547350-b0360980-a4c7-11ea-8a5b-f30013d2cb0f.png)

The main characteristics of a tank drive are the wheels set up in a box, with all being parallel.

**Use Cases**: The Tank Drive is incredibly common in all disciplines of robotics, it is relatively simple and incredibly easy to maintain. If you are a beginner, it is highly recommended that you get familiar with this type of drive. 

**Disadvantages**: The primary disadvantage to the Tank Drive is the mobility outside of going forward and backward.

# Holonomic Drivetrains

## Mecanum Wheel Drive
Mecanum Wheels are a confusing sight to see, however the design and programming are both quite simple. 

![Mecanum Drive](https://user-images.githubusercontent.com/65926085/83550465-8206f880-a4cc-11ea-87b7-bb26af8c5626.png)

Mecanum Drives are constructed exactly the same as a Tank Drive, except the wheels have an additional functionality of horizontal movement. 

**Use Cases**: A Mecanum Drive is incredibly useful as it allows horizontal movement with only 4 motors required. It is a logical step forward from the Tank Drive, as it operates under mostly the same principles.

**Disadvantages**: The primary disadvantage to a Mecanum Drive is the large size of wheels. Especially on a limited size robot, these can take up a large amount of space. Each wheel also must be powered individually, which can lead to more mechanical complexity. While performing horizontal movement, the robot is not able to move vertical.

## H-Drive / Strafe Wheel Drive
This type of drive relies on a 5th wheel in the center of a drive in order to create horizontal motion. 

![H-Drive](https://user-images.githubusercontent.com/65926085/83558236-5558de00-a4d8-11ea-9052-47b3f9ea525f.png)

H-Drives have an identical base to the Tank Drive, however all wheels are omni-directional, and a single wheel is added in the exact center.

**Use Cases**: The H-Drive has one major advantage, it allows the robot to translate in any direction, including diagonals. This is surprisingly useful for manuvering around a field at the same orientation.

**Disadvantages**: The major disadvantage comes with motor designation, as an odd number of motors is required to make this drive type function. With a limit on the amount of motors, it can occasionally be difficult to design around an odd number of motors.

## X-Drive
Continuing on the single letter designations for drive types, the X-Drive allows for many of the advantages of holonomic drives without some of the drawbacks.

![X-Drive](https://user-images.githubusercontent.com/65926085/83556810-2a6d8a80-a4d6-11ea-9a5f-f44a0f9f7698.png)

The X-Drive is unlike every other drive. Each wheel is at a 45 degree angle to the forward direction of the robot. Wheels that are in opposite corners are parallel, while adjacent wheels are perpendicular.

**Use Cases**: X-Drives have the ability to translate in any direction, much like the H-Drive, and still needing only 4 motors for the drive. It is also the most space efficient holonomic design.

**Disadvantages**:An X-Drive requires a 45 degree angle, small imperfections in the build can lead to errors while in operation. The programming can also be difficult to comprehend at first, especially relating to moving not in the cardinal directions. 

# VEXU/VAIC Holonomic Drivetrains
Due to either motor limit, or complexity in parts. These drive trains are not feasible to build in the standard VRC environment. However, they can be made to work in VEXU/VAIC.

## Swerve Drive
The Swerve Drive is the most conventional method to having holonomic movement.

%% insert Normal Swerve CAD (maybe even VEXU specifications)

Each individual wheel is directly powered by one motor and have a secondary motor controlling the direction of each wheel.

**Use Cases**: Swerve Drives are common to have static wheels move in a holonomic format. 

**Disadvantages**: Due to the minimal motor count being 8, this design is not useful in the VRC discipline. It is also quite bulky and requires a large amount of focus to be placed on base design. 

## Differential Swerve Drive
A variation of the Swerve Drive, the differential allows the robot to increase the power of each individual wheel for the same number of motors.

%% insert Michael/Sam's Differential Swerve

Each Wheel has two motors powering two separate ring gears. While the ring gears move in opposite directions, the Wheel will move as normal. However when the ring gears are moving in the same direction, the Wheel rotates it's orientation.

**Use Cases**: Differential Swerves are one of the most useful types of drivetrain when done properly. They can provide ample speed and traction in any direction and allow for incredibly complex movement while maintaining a constant robot orientation.

**Disadvantages**: This drive type is incredibly complex, requiring a large amount of 3D printed parts and extensive programming knowledge. 

### Contributions:

Thomas Kelleher
Michigan Task Based Robotics

