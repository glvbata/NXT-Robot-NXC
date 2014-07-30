NXT-Robot-NXC
=============

An NXT robot programmed in NXC


Objective: The robot will explore the lab by wandering randomly. It will look for white patches/lines which will represent "food". It will react to objects that it bumps against. It will detect and approach objects. It will also attempt to escape from bright flashes of light which it will interpret as a possible threat. 

The robot is programmed to have 7 different behaviors: 

1.) Wander - The robot wanders randomly.

2.) Object Detection and Approach - If the robot detects an object, it will approach it.

3.) Avoid Obstacles - It will avoid obstacles when encountered. 

4.) Gradient Following -  The robot must determine the direction it should follow to get to the food patch by detecting the gradient (increasing width of the line) and following it to find the patch.

5.) Patch Feeding - Once a robot is in a patch it should not leave unless it detects an object, is frightened by a flash of light, or has fed until it is “full”. If it feeds until it is “full”, it must return to wandering. While the robot is feeding, a variable called "energy_level" should be incremented. If the robot feeds for a full two minutes this variable should be at its maximum “full” value. After the robot leaves the patch, for whatever reason, this variable should decrement slowly. Low values for this variable are interpreted as "hunger". When the energy variable is below a certain point (no more than two minutes after feeding) the robot should be ready to feed again “hungry”. Feeding involves continuously moving in a non-repetitive way (wandering) on the patch.

6.) Escape - The robot dislikes bright flashes of light and considers them a threat.

7.) Death - If a robot's "energy_level" variable ever reaches 0, the robot is “dead” and should cease all activity after emitting a final sound.

