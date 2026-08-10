# Echoed Nights

A **first-person psychological horror game** built in Unity with C#, featuring reactive enemy AI, dynamic environmental storytelling, and a looping nightmare atmosphere. Built as my graduate capstone at Saint Martin's University and published on Steam.

**[▶ Echoed Nights on Steam](https://store.steampowered.com/app/4340810/Echoed_Nights/)**

> ### 📄 This repository is the project record, not the source code
>
> The Unity project is not published here. What this repo holds is the written and visual record of the project:
>
> | File | What it is |
> |---|---|
> | [`MSCS-ProjectReport-Landon.pdf`](MSCS-ProjectReport-Landon.pdf) | The capstone report — design, AI architecture, methodology, QA, and results |
> | [`Echoed Nights.pptx`](Echoed%20Nights.pptx) | The capstone defense presentation |
> | [`screenshots/`](screenshots) | Gameplay captures from the shipped build |
>
> If you came here for code, this isn't that repo — read the report instead. The evidence for this project is a game that shipped and a document that explains how it was built.

> ⚠️ **Development note:** Several features and mechanics changed significantly between the documented design and release.
>
> Notable example: enemy AI was originally architected using **reinforcement learning** — training agents through environmental simulations. This approach was scoped down due to the computational resources required to run sufficient training simulations. The shipped game uses **NavMesh pathfinding with a finite state machine**, which proved more stable and performant within the project's constraints. The report is preserved as a record of the full development process, including early design decisions and architectural exploration.

## Screenshots

| | | |
|---|---|---|
| ![Hallway](screenshots/gameplay-1.png) | ![Corridor](screenshots/gameplay-2.png) | ![Event Room](screenshots/gameplay-3.png) |

> **Role:** Lead Developer & Director  
> **Team:** Solo / small team  
> **Duration:** 2023 - 2024

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

Developed as a graduate capstone project at **Saint Martin's University** (M.S. Computer Science, completed May 2024). The [project report](MSCS-ProjectReport-Landon.pdf) in this repository is the full written research report on AI agent design in game environments.

---

**Developer:** Landon Armstrong | [GitHub](https://github.com/Larmstrong1127) | [LinkedIn](https://linkedin.com/in/landon-armstrong)
