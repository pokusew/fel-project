# NAME

**Possible names:**
* Porting autonomous software/driving stack of F1/10 model car to ROS 2
* Using ROS 2 on the autonomous F1/10 model car
* Migration
* Migrating

**Useful vocabulary:**
* The goal of this project is to ... and ...
* goal, aim
* outcome, result
* present, introduce
* describe, cover
* implement
* study, explore
* deal with, focus, cover
* propose, suggest, come up with
* verify, compare
* groundwork
* The project lays the foundations for future migration


## Abstract

The new version of the Robot Operating System – ROS 2 – brings significant improvements over its predecessor
ROS 1. We describe both versions and compare their differences. Then we cover the process of migrating a ROS 1
application to ROS 2 on the example of the Follow the Gap app that is part of CTU's F1/10 project. In the next
part, we focus on setting up an NVIDIA Jetson TX2 module so that it can run ROS 2 applications and provide
good developer experience in environments where Jetson module is shared among many students and researches.
The first result of this project is a ROS 2 port of the Follow the Gap application. Its working is
demonstrated in the Stage simulator on Ubuntu and macOS. The second result is a setup guide for NVIDIA Jetson
TX2 that covers creating a fully-setup OS image with ROS 2 on a bootable SD card. The last result is a
collection of setup guides and documentation that cover various aspects of working with ROS.


## Keywords

ROS, ROS 1, ROS 2, ROS 2 migration, F1/10, Follow the Gap, autonomous model car, NVIDIA Jetson TX2


---


# Introduction

Since the Robot Operating System was started in 2007, it has gained great popularity and has become the
standard in robotics community. However, it has turned out that the original architecture ROS has many
limitations (concerning mainly performance, efficiency and real-time safety). Thus, a new version of ROS – ROS
2 – has been designed from ground up to allow more use-cases and solve pain points of ROS 1. Missing features
and incompatible packages have been slowing down the adoption of ROS 2 since its first public release in 2017.
But in recent years, the situation has improved a lot and the adoption of ROS 2 has accelerated. Thus, now it
is the right time start migrating applications from ROS 1 to ROS 2 and benefit from new possibilities.

The F1/10 platform is scaled-down (1:10) model of an autonomous car that originates from F1/10 Autonomous
Racing Competition. Thanks to its affordability, the platform can be used for development, testing and
verification of autonomous driving systems and related algorithms. At CTU, multiple F1/10 models have been
created and used (TODO: links). Currently, all of them are based on NVIDIA Jetson computing modules and
powered by ROS 1 Kinetic Kame.

The goal of this project is to migrate a selected part of the CTU's F1/10 project from ROS 1 Kinetic Kame to
ROS 2 Foxy Fitzroy. The result should be a working port running on ROS 2 in a simulator and on a physical
model car with NVIDIA Jetson computing module.

In the second chapter, both versions of ROS are described and ROS 2 and its differences to ROS 1 are studied.

In the third chapter, the software and hardware stack of CTU's F1/10 project is introduced. Then the Follow
the Gap application is selected for migration to ROS 2. The migration is described. The result

The fourth chapter focuses on setting up an NVIDIA Jetson TX2 module so that it can run ROS 2 applications.
The emphasis is given on providing a good developer experience in environments where the Jetson module is
shared among many students and researches. Thus, boot options of the Jetson modules are explored. Then a
solution with a bootable SD card is presented.

Finally, the achieved results are summarized in the last chapter.


# Robot Operating System

“a set of software libraries and tools for building robot applications“ [[3]][3]

The Robot Operating System (or ROS) is “an open-source, meta-operating system” [[1]][1]
that consists of “tools, libraries, and conventions that aim to simplify the task of creating complex and
robust robot applications across a wide variety of robotic platforms“ [[2]][2].

## ROS Computation Graph

## ROS 1

build system is catkin, catkin_make, catkin_make, catkin_make_isolated, catkin_tools


## ROS 2

distributed, based on DDS
build system is ament, build tool colcon

## Migration

ROS dates back

A typical ROS application


Since ROS was started in 2007, a lot has changed in the robotics and ROS community. The goal of the ROS 2
project is to adapt to these changes, leveraging what is great about ROS 1 and improving what isn’t.

(potentially distributed across machines)

ROS applications are written in a distributed-fashion.

A typical ROS application is split up into loosely coupled process (so called nodes)

The Robot Operating System (or ROS) is

Application is split up into multiple computation nodes that commonunitces togethers.

it allows code decoupling and sharing.

TODO

A typical ROS application


# F1/10 platform

TODO


# NVIDIA Jetson TX2

TODO

## Initial Setup

## Building ROS 2 from sources

## Running the Follow the Gap Demo

## Bootable SD Card


# Conclusion

TODO

documentation created

should be pretty straightforward missing pieces, Orbitty carrier setup, porting of HW packages

analysis of real-time properties, temporal determinism, communication overheads, performance, in particular
when compared with the ROS 1


# References

[1]: http://wiki.ros.org/ROS/Introduction

[2]: https://www.ros.org/about-ros/

[3]: https://docs.ros.org/en/foxy/index.html

[4]: https://www.ros.org/history/

[5]: https://design.ros2.org/articles/why_ros2.html
