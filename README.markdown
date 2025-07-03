# Operation Clean Sweep

## 🎮 Overview

**Operation Clean Sweep** is a 3D third-person shooter (TPS) game with a first-person mode toggle, developed using Unreal Engine 5. It is built as part of the Data Structures & Algorithms (DSA) course project. The game places players in a tactical team of four (player + bots or multiplayer), storming an enemy HQ defended by AI enemies. It blends intense combat, squad coordination, and DSA-powered systems.

---

## ✨ Features

### 🔫 Player Mechanics

- Smooth 3rd person movement with jumping, crouch, and slide
- Toggle between TPS and FPS views (scoped view enters FPS)
- Shooting with bullet impact visuals, recoil animations, muzzle flash
- Health bar system with limited healing

### 🧑‍🤝‍🧑 Team Mechanics

- Team of 4 (1 player + 3 bots / multiplayer optional)
- Real-time team stats (Kills, Damage, Status) via Tab menu

### 🧠 Enemy AI

- AI patrol, alert, shoot, and take damage
- Health, death, and behavior tree logic

### 🌍 Environment

- Large terrain-based map (forest, river, mountain-boundary)
- Water acts as a death zone
- Central enemy HQ as the mission objective

### 🧪 Game Systems

- Player/enemy spawning logic
- Win condition: eliminate all enemies at HQ
- UI: Health, Ammo, Objective tracker, Team stats (TAB)

---

## 🧮 DSA Concepts Implemented

| Concept | Use Case |
| --- | --- |
| Arrays/Lists | Manage team stats, enemy pools, bullets |
| Queues | Cooldowns, spawn queue |
| Graphs | AI navigation using NavMesh |
| Trees | AI behavior tree logic |
| Maps | Track kills, damage per teammate |
| State Machines | Player states, game mode transitions |

---

## 📁 Project Structure (In GitHub)

```
Operation-Clean-Sweep/
├── README.md
├── LICENSE
├── docs/
│   ├── GameDesignDocument.md
│   ├── SprintPlan.md
│   ├── ProjectProposal.pdf
│   └── NotionLinks.md 
└── assets/
    ├── characters/
    ├── maps/
    └── UI/
```

⚠️ **Note**: Source code will not be added directly to this repo. It will be shared via a secured Google Drive link after completion.

---

## 🔗 Notion Workspace & Documentation

- Full documentation, GDD, and progress tracker is maintained via Notion.
- 🌐 Operation Clean Sweep - Project Hub

---

## 🗂️ Downloads & Demos

- 📂 Google Drive Link – Final Project Files *(replace after completion)*
- 📹 Gameplay demo video will be added post-development
- 📸 Screenshots to be added once core gameplay is functional

---

## 👥 Team

| Name | Role | Contributions |
| --- | --- | --- |
| **Muhammad Affan Bin Aamir** | Project Lead, Gameplay Developer | Core logic, shooting, DSA integration, GitHub, Planning |
| **Muhammad Umar** | Map & Asset Manager | Models/maps research, Blueprint setup, Visual adjustments |

---

## 🧪 Development Timeline (Sprints)

| Sprint | Focus |
| --- | --- |
| Sprint 1 | UE5 Setup, Basic Controls |
| Sprint 2 | Player Shooting, Health, Slide, Scope |
| Sprint 3 | AI Integration, Map Setup |
| Sprint 4 | DSA Integration, UI, Tab Menu |
| Sprint 5 | Final Polish, Testing, Docs, Demo Video |

---

## 🧾 License

This project is licensed under the MIT License. See the LICENSE file for details.