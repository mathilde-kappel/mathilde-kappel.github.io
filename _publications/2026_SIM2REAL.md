---
title: "A Sim-to-Real Integration Pipeline for Training and Deployment of Chunk-Based VLA Manipulation Policies"
collection: publications
category: Workshops
permalink: /publication/2026-ros2-architecture-articulated-object-manipulation
header:
  teaser: vignette_sim2_real.png
excerpt: >-
  Vision-Language-Action (VLA) models have become a prominent paradigm for mapping multimodal inputs, including semantic instructions, visual observations of the scene, and proprioceptive observations, to robot actions. Most state-of-the-art models predict actions in the end-effector pose space as sequences of action chunks. Training and evaluating these models requires large-scale collections of real-world demonstrations, pairing robot actions with the corresponding visual and proprioceptive observations. Collecting such data on real hardware typically relies on human teleoperation, making the process costly, time-consuming, and difficult to scale. We present an open-source sim-to-real experimental protocol that addresses this bottleneck: expert trajectories generated in simulation are replayed open-loop on a real Franka FR3 setup, where the corresponding real visual and proprioceptive observations are recorded and converted into a format compatible with VLA training. The same deployment stack is then reused, in closed-loop, to evaluate a trained policy on that setup, so that data collection and evaluation share an identical hardware configuration.
date: 2026-06-24
venue: 'Workshop IROS 2026, Sim2Real and Classical Control: From Rigorous Theory to Data-Driven Robotics'
paperurl: 'https://arxiv.org/abs/2609.21817'
posterurl: '/files/Horizontal_IROS_Workshop_sim2real_poster_mathilde.pdf'
citation: 'Kappel, M., Grislain, C., Chetouani, M., Sigaud, O., Annabi, L., Ben Amar, F., Doncieux, S., & Khoramshahi, M. (2026). ROS2 Architecture for Articulated Object Manipulation Using Trajectory Primitives Learned in Simulation. Technical report, Sorbonne University.'
---

**Abstract:** The work presented in this document focuses on the ROS2 integration of expert trajectories learned in simulation. It enables robotic manipulation of articulated objects in an open environment. The proposed architecture relies on two complementary methodologies. First, a preliminary offline learning module generates trajectory primitives using the Genesis physics simulator. Then, an online module selects and executes the optimal simulated trajectory to solve a given task in a specific real-world scenario. This document also includes the results and observations from the experimental deployment of this approach. The project web page, containing the code and documentation, is available at https://kappel.web.isir.upmc.fr/trajectory_primitive_website/.
