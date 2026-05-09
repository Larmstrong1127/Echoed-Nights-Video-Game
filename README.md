# Echoed Nights

A **first-person psychological horror game** built in Unity with C#, featuring reactive enemy AI, dynamic environmental storytelling, and a looping nightmare atmosphere.

> **Role:** Lead Developer & Director  
> **Team:** Solo / small team  
> **Duration:** 2022 - 2023

## Overview

Echoed Nights puts the player in a dark, shifting environment where they must navigate terror while being hunted by intelligent AI enemies. The project demonstrates end-to-end game development — from initial design documentation through final quality assurance.

## Key Features

- **Enemy AI System** — NavMesh pathfinding combined with finite state machines produces fluid, reactive enemy behavior that responds dynamically to player actions
- **Dynamic Difficulty** — enemy aggression and patrol patterns shift based on player performance
- **Environmental Storytelling** — atmospheric sound design, lighting, and environmental cues drive the horror experience without heavy exposition
- **Full Project Lifecycle** — bi-weekly stakeholder reviews, milestone tracking, and structured QA process from design through delivery

## Tech Stack

| | |
|---|---|
| Engine | Unity |
| Language | C# |
| AI | NavMesh Pathfinding, Finite State Machines |
| Physics | Unity Rigidbody, Collider system |
| Audio | Unity Audio Mixer |
| Version Control | Git / GitHub |

## AI Architecture

Enemy agents use a **finite state machine (FSM)** with four primary states:

| State | Behavior |
|---|---|
| Patrol | Follows waypoints when no player detected |
| Alert | Investigates sounds or peripheral movement |
| Chase | Pursues player at full speed when line-of-sight confirmed |
| Search | Sweeps last known player position after losing track |

NavMesh handles real-time pathfinding and obstacle avoidance, ensuring enemies navigate complex geometry without clipping or getting stuck.

## Academic Context

Developed as a graduate capstone project at **Saint Martin's University** (M.S. Computer Science, 2023). Includes full project documentation and a written research report on AI agent design in game environments.

---

**Developer:** Landon Armstrong | [GitHub](https://github.com/Larmstrong1127) | [LinkedIn](https://linkedin.com/in/landon-armstrong)
