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

## Mecanum Drive

![Mecanum Drive](https://user-images.githubusercontent.com/65926085/83550465-8206f880-a4cc-11ea-87b7-bb26af8c5626.png)

The Mecanum Drive is just as simple to build as the Tank Drive, but has the ability to drive sideways. It uses Vex Mecanum wheels in order to drive, turn, and strafe.

**Advantages and Disadvantages:** The Mecanum Drive is simple to build and, while mecanum wheels are thicker than omni wheels, it takes up little space. The Mecanum Drive is also difficult to push from the side, however it strafes more slowly than it drives forward. Because Vex mecanum wheels have only 7 sets of rollers, driving is often "clunky", which is a disadvantage when programming autonomous functions using the integrated motor encoders.

![7K&apos;s Mecanum Drive](https://user-images.githubusercontent.com/65926085/83552256-14100080-a4cf-11ea-8362-56dd9513c343.png)

The Mecanum Drive was utilized by [7K's Tower Takeover Robot](https://www.youtube.com/watch?v=vGkMw4Nx-Ks). Mecanum wheels are especially effective in games like Tower Takeover which involve rows of game elements or aligning with the field perimeter.

**NOTE:** When building a Mecanum Drive, the wheels must be orientated in a certain manner to allow for strafing. The most common setup involves the top rollers of the wheels forming and "x" shape as shown above. The important thing here is that wheels in opposite corners have their rollers pointing in the same direction.

## X-Drive

![X-Drive](https://user-images.githubusercontent.com/65926085/83556810-2a6d8a80-a4d6-11ea-9a5f-f44a0f9f7698.png)

The X-Drive is a bit more complex to build than either the Tank or Mecanum Drives, but it allows for greater maneuverability than the Mecanum Drive.

**Advantages and Disadvantages:** The X-Drive is the most maneuverable Vex drivetrain and, unlike the Mecanum Drive, its forward speed is equal to its sideways speed. However, the wheel assemblies take up quite a bit of room on a robot, leaving less space for mechanisms.

One interesting thing to note about the X-Drive is its speed compared to a tank drive. Given a tank drive and an X-Drive with the same wheel size and motor cartridges, the X-Drive has a higher maximum speed. The math behind this is shown in [this article by AURA](https://aura.org.nz/why-is-x-drive-faster/).

This is a [Simpler X-Drive Design](https://www.vexforum.com/t/simpler-x-drive-design/80770) which uses metal attached at an angle rather than 45 degree angle brackets:

![Simpler X-Drive](https://user-images.githubusercontent.com/65926085/83553426-cd230a80-a4d0-11ea-8731-be887931df6d.png)

It is also a viable option when creating an X-Drive.

**NOTE:** When building an X-Drive, it is best to position the wheels in a square shape \(i.e. the vertical distance between wheel centers is equal to the horizontal distance between wheel centers\). Although other configurations will work, arranging the wheels in a square creates the optimal maneuverability and turning.

## H-Drive

![H-Drive](https://user-images.githubusercontent.com/65926085/83558236-5558de00-a4d8-11ea-9052-47b3f9ea525f.png)

The H-Drive is constructed very similarly to the Tank Drive. However, it contains a wheel in the center of the robot which both allows for strafing and prevents being pushed from the side. This is not a common drivetrain choice, but can be a viable one.

**Advantages and Disadvantages:** The H-Drive has more maneuverability and can resist pushing from the side more effectively than the Tank Drive due to its extra strafe wheel. However, its sideways motion is generally either slower or weaker than its forward motion. In addition, it takes an extra motor to power the center wheel. This takes away one motor from mechanisms, which is often not worth the tradeoff.

![99904A&apos;s H-Drive](https://user-images.githubusercontent.com/65926085/83677779-450d3580-a5a2-11ea-9238-1f288bbdf526.png)

The H-Drive was utilized by [99904A's Turning Point Robot](https://www.youtube.com/watch?v=MLQynFXRzZI) to complement their sideways catapult.

**NOTE:** When building an H-Drive, it is crucial that the center wheel contact the field in roughly the same manner as the other four. To accomplish this, the mounting for this wheel can be spaced down slightly, or a tensioning system can be used to pull the center wheel into the ground.

## Building a Drivetrain

The performance of any drivetrain is based not only on the type selected, but also on the quality with which it is designed and built. This Vex Forum thread on [Designing a Quality Drive](https://www.vexforum.com/t/designing-a-quality-drive/81850) is a great resource for newer teams interested in maximizing their drive's performance.

There are 4 main components to designing and building a quality drive:

* **Planning:** Set constraints for your drive to best accomplish the tasks in the game \(i.e. "The width must be less than 13 inches." or "There must be at least 6 inches of room on the front of the drive to attach a mechanism\). By setting these constraints before you begin designing, you'll have a much easier time later on. 
* **Designing:** CAD tools such as [Autodesk Fusion 360](https://www.autodesk.com/products/fusion-360/students-teachers-educators) are especially helpful when designing your drivetrain, as they allow you to visualize the drive in its final form. However, a pen and some graph paper is always an acceptable alternative. Whatever the method, fully designing the drivetrain before beginning the build is very beneficial.
* **Robustness:** Make sure that your design contains bracing in several places to make a more robust drivetrain. A simple test to determine whether the frame is robust enough is to try to bend it diagonally. If it bends easily, or very far, more bracing should be utilized. One technique to increase a drivetrain's robustness involves placing spacers between opposite sides of a C-channel being attached, as shown [here](https://www.vexforum.com/uploads/default/original/3X/7/6/76ca8cbde060b57aa60ade37a45e920d7cbdaada.png). For a 1x2x1 C-channel, a .375" spacer and a .5" spacer fit snugly between the sides of the channel.
* **Efficiency:** Ensure that each wheel assembly \(and gear or chain assembly, if your drive utilizes these\) has as little friction as possible. A good rule of thumb is that if a mechanism can spin freely for more than 5 revolutions, it has minimal friction. Of course, you are the judge of whether or not your mechanisms cause friction, and how much this affects your build. Some common causes of unwanted friction include misalignment \(components are not in line, causing rotation to be more difficult\) and rubbing \(two components are moving against each other; they should be spaced apart\).

### Contributing Teams to this Article:

* [2775J](https://www.youtube.com/channel/UCxpfFq6ShDvgmU9P4y6rc_Q?view_as=subscriber) \(Jackson Area Robotics\)

