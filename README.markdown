# Operation Clean Sweep

## 🎮 Overview

**Operation Clean Sweep** is a 3D tactical third-person shooter (TPS) with a first-person (FPS) toggle, built using Unreal Engine 5 as part of a Data Structures & Algorithms (DSA) course project. Players lead a 4-member squad (1 player + 3 AI bots, with multiplayer as a stretch goal) to infiltrate and capture an enemy HQ guarded by 25 AI bots, followed by 15 reinforcements. The game blends intense combat, squad coordination, and DSA-powered systems, featuring a dynamic map with a mini-map, limited healing/ammo pickups, and spectator mode.

- **Genre**: Tactical Shooter (TPS/FPS Hybrid)
- **Platform**: PC
- **Engine**: Unreal Engine 5 (C++ with Blueprints)
- **Timeline**: July 5, 2025 – August 29, 2025
- **MVP Target**: August 22, 2025 (Feature Freeze)

## ✨ Features

### 🔫 Player Mechanics

- Smooth TPS movement (walk, sprint, crouch, prone, jump, slide)
- Toggle between TPS and FPS views (scoped aim in FPS)
- Shooting with hip fire spread, recoil, muzzle flash, bullet impact
- Health system with limited healing (20–25 HP from pickups)
- Weapons: AR (300 rounds), pistol (50 rounds), knife; ammo pickups

### 🧑‍🤝‍🧑 Team Mechanics

- 4-player squad (1 player + 3 AI bots)
- Real-time stats via Tab menu (name, kills, points, assists, alive/dead)
- Spectator mode: switch to teammate camera on death

### 🧠 Enemy AI

- 25 initial bots + 15 reinforcements (7 + 8 sides) with patrol, alert, attack
- Behavior Trees, health, death, movement (run, crouch, slide)

### 🌍 Environment

- Terrain-based map (forest, river death zone, unclimbable mountains)
- Central enemy HQ as the mission objective
- Ammo boxes and limited healing items on furniture

### 🧪 Game Systems

- Win condition: eliminate all 40 enemies
- Loss condition: squad death
- Pause/resume functionality
- UI: Health/Ammo HUD, mission box (via 'Alt'), mini-map (expandable via 'M')

## 🧮 DSA Concepts Implemented

| Concept | Use Case |
| --- | --- |
| Arrays | Manage squad members, enemy pools, bullet tracking |
| Queues | Cooldowns, spawn timers, reinforcement scheduling |
| Stacks | Undo player actions, recent damage event tracking |
| Linked Lists | Dynamic lists of active AI bots or ammo pickups |
| Trees | Behavior Trees for AI logic |
| Graphs | NavMesh for AI pathfinding |
| Hash Maps | Track kills, points, assists, damage stats |
| State Machines | Player states (idle, shooting, sprinting), game states |

## 📁 Project Structure (In GitHub)

```
Operation-Clean-Sweep/
├── README.md
├── LICENSE
├── docs/
│   ├── GameDesignDocument.md
│   ├── SprintPlan.md
│   ├── TechSpecs.md
│   ├── RiskDependencyLog.md
│   ├── MVPChecklist.md
│   ├── MilestoneTimeline.md
│   └── ProjectProposal.pdf
└── assets/
    ├── characters/
    ├── maps/
    └── UI/
```

⚠️ **Note**: Source code and assets are stored in Google Drive (not public on GitHub). A link will be added post-completion.

## 🚀 Getting Started

### Prerequisites

- **OS**: Windows 10 (64-bit)
- **CPU**: Intel Core i5-7400 / AMD Ryzen 5 1400 or better
- **RAM**: 8 GB (16 GB recommended)
- **GPU**: NVIDIA GTX 1050 Ti / AMD RX 560 (2-4 GB VRAM) or better
- **Storage**: 20 GB free (SSD preferred)
- **Software**: Unreal Engine 5.6, Visual Studio 2022, Git

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Afffan16/OperationCleanSweep.git
   ```
2. Install Unreal Engine 5.6 from the Epic Games Launcher.
3. Open the `.uproject` file in the root directory with Unreal Engine.
4. Download dependencies (e.g., Marketplace assets) via the Unreal Editor.

### Running the Game

- Build the project in Visual Studio (Development Editor configuration).
- Launch from Unreal Editor or the generated executable.
- Use default keybindings: WASD (movement), Left Click (shoot), Tab (stats), M (mini-map).

## 🛠 Development Details

### Tools

- **Engine**: Unreal Engine 5
- **Programming**: C++ (core logic), Blueprints (visual scripting)
- **Assets**: Unreal Marketplace, Mixamo, Quixel
- **Version Control**: GitHub
- **Documentation**: Notion
- **Storage**: Google Drive

### Team

| Name | Role | Contributions |
| --- | --- | --- |
| **Muhammad Affan Bin Aamir** | Project Lead, Gameplay Developer | Core logic, shooting, DSA integration, planning |
| **Muhammad Umar** | Map & Asset Manager | Models/maps research, Blueprint setup, visuals |

### Status

- **Start Date**: July 5, 2025
- **Current Phase**: Planning (as of Jul 3, 2025, 09:15 PM PKT)
- **Final Delivery**: August 29, 2025 (Demo Video + Documentation)

## 🗓 Development Timeline (Sprints)

| Sprint | Duration | Focus |
| --- | --- | --- |
| Sprint 1 | Jul 5–11 | UE5 Setup, TPS Movement |
| Sprint 2 | Jul 12–18 | Combat, Health, Weapons |
| Sprint 3 | Jul 19–25 | AI, Initial Map |
| Sprint 4 | Jul 26–Aug 1 | Map Enhancements, Mini-Map |
| Sprint 5 | Aug 2–8 | UI, Team Stats, Spectator Mode |
| Sprint 6 | Aug 9–15 | Reinforcements, Game States, Pause |
| Sprint 7 | Aug 16–22 | Objective Logic, Testing |
| Sprint 8 | Aug 23–29 | Polish, Demo, Documentation |

## 📚 Documentation & Resources

- 🌐 **Notion Workspace**: Operation Clean Sweep - Project Hub
- **🗃️ Google Drive**: (Link to be added post-completion for source files and assets)
- 📂 **Planning Documents**: Check the docs/ folder for detailed plans

## 📥 Downloads & Demos

- 📹 Gameplay demo video will be added post-development
- 📸 Screenshots to be added once core gameplay is functional

## 🤝 Contributing

This is a collaborative project between Affan and Umar. External contributions are not currently accepted, but feedback is welcome via the Notion workspace or GitHub Issues.

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.