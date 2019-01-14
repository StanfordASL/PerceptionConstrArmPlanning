# Perception Constrained Robot Manipulator Planning
Code for "Perception-Constrained Robot Manipulator Planning for Satellite Servicing," by Tariq Zahroof, Andrew Bylard, Hesham Shageer, and Marco Pavone.

This repository contains references to two packages (git submodules):
1. The modified moveit package with perception constraints
2. The motoman package with robot examples

- Download the submodules linked in this repository by typing the following within this repository
```
$ git submodule init
$ git submodule update
```

- Follow the instructions in "Restore_L_MoveIt_Documentation.pdf" to set up moveit and anxilliary packages.
- Then, move both packages from this repository to your catkin workspace directory. Don't forget to replace the native moveit package with this build's custom package


- The motoman_sia20d_moveit_updated package features the code from the paper. Type the following to execute:

```$ roslaunch motoman_sia20d_moveit_updated camera_navigation.launch ```

- Additionally, code for a trajectory optimizer (with robot singularities) was included. Type to launch:

```$ roslaunch motoman_sia20d_moveit_updated trajectory_viewer.launch ```
