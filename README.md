---
classes: wide
---
The Biped Open Platform Project started with the idea to create an affordable yet capable platform for research in robotics and 2-legged locomotion. The components are mostly either 3d-printable, open-source, or off-the-shelf hardware. We're just getting started! At present, the project is in an early and untested stage, with many parts still undergoing actively design, testing, and changes. We make both early concepts and current versions available to allow reproduction, contributions, or spin-off projects. If you like or use this project, we'd love to hear about it!

### Philosophy and related projects

Humanoid robots that are suitable for research are expensive: even open-sourced platforms will easily be in excess of $20k. For walking robots, in the last years a number of quadruped platforms have become known for their abilities to walk and jump, using relatively inexpensive brushless (BLDC) motors. Some biped robots using similar ideas also exist, though there are fewer of them, and here is where the Biped Open Platform Project aims to contribute, by providing a (relatively) easy to reproduce affordable research robot. Here are some of the core ideas:

#### A hybrid serial-parallel leg design
This idea is from a group at Disney Research, by Kevin Gim et al. - a [serial-parallel leg design](https://la.disneyresearch.com/publication/design-and-fabrication-of-a-bipedal-robot-using-serial-parallel-hybrid-leg-mechanism/) that allows most of the actuators to be placed in the hip (there are no motors in the knee, and only one motor in each foot), resulting in a lighter structure. The robot introduced in their paper is relatively small, making use of servo motors. For the larger size design in our project, we replace the servos with BLDC motors.

#### Open source commercially available motor controllers
The [mjbots](https://mjbots.com) moteus boards are open-source controllers for BLDC motors designed for legged robotics projects. They are an affordable solution to connect standard brushless motors, and allow to chain them up using a CAN bus. This also means it is not required to design any own controller boards: the electronics aspects of the project reduce to connecting or soldering a few wires.

#### Other open-source robotics projects
The [Open Dynamic Robot Initiative](https://open-dynamic-robot-initiative.github.io) is an open-source robotics project that helped to encourage the open-sourcing of this project. In terms of development, the ODRI is a few years ahead of this project, with an excellent documentation and quality of the design. We recommend having a look. ODRI follows a very modular design, and includes their own motor controller. Our Biped Open Platform Project uses an off-the-shelf controller instead, but took inspiration at some of parts of their design.  
