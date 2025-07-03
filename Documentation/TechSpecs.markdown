# Technical Specification Document

## 🎮 Project Title: Operation Clean Sweep

## 📌 Purpose

This document outlines the technical architecture, development tools, software structure, and system requirements for the Operation Clean Sweep project.

## 🧱 Architecture Overview

| Layer | Description |
| --- | --- |
| Game Logic | Written in C++ using Unreal Engine 5 (UE5) |
| Visual Scripting | Blueprints used for prototyping and simple visual features (by Umar) |
| UI Layer | UMG for HUD elements (health, ammo, objectives, team stats, mini-map) |
| AI Layer | UE5 Behavior Tree system (Blackboard, NavMesh, Patrol, Alert, Shoot states) |
| Animation Layer | Animation Blueprints for slide, crouch, prone, shoot, death |
| Data Structures | C++ DSA implementations (arrays, queues, stacks, linked lists, graphs, trees, hash maps, state machines) for managing stats & logic |

## 🛠 Development Stack

| Component | Technology | Notes |
| --- | --- | --- |
| Game Engine | Unreal Engine 5 | C++ project template, uses third-person base |
| Programming | C++ | Core game mechanics |
| Visual Logic | Blueprints | UI, animation transitions, map assets |
| 3D Assets | UE Marketplace / Mixamo | Map, weapons, AI bots |
| UI Design | UMG (Unreal Motion Graphics) | Health bar, scope UI, tab screen, mini-map |
| Version Control | GitHub | Repo contains docs, asset logs, project logs |
| Documentation | Notion + GitHub | Task board, sprint plan, design documents |
| External Storage | Google Drive | Project source files (C++ + .uproject), assets |

## 🧠 Core Systems and Features

### Player Mechanics

- Movement: walk, sprint, crouch, prone, jump, slide
- Shooting: recoil, hip fire with spread, scoped FPS view, animations
- Health: limited healing from pickups, death with spectator mode
- Weapons: AR (300 rounds), pistol (50 rounds), knife; ammo pickups

### AI Mechanics

- 25 initial bots + 15 reinforcements (7 + 8 sides) with patrol, alert, attack
- Behavior Trees, damage, death, movement (run, crouch, slide)

### UI Features

- Health bar, ammo count, mission box (via 'Alt'), objective prompt
- Tab Menu: team stats (name, kills, points, assists, alive/dead)
- Mini-map (limited circle, expandable via 'M')

### DSA Logic

- Arrays: Squad members, enemy/bullet pooling
- Queues: Spawn timers, healing cooldowns, reinforcement scheduling
- Stacks: Undo player actions, recent damage event tracking
- Linked Lists: Dynamic lists of active AI bots or ammo pickups
- Graphs: NavMesh navigation for AI pathfinding
- Trees: Behavior Trees for enemy AI logic
- Hash Maps: Kill tracking, points, assists, damage stats
- State Machines: Player states (idle, shooting, sprinting, prone), game states

## 🧾 Folder Structure (Planned GitHub Structure)

```
Operation-Clean-Sweep/
├── README.md
├── LICENSE
├── docs/
│   ├── GameDesignDocument.md
│   ├── SprintPlan.md
│   ├── TechSpecs.md
│   └── ProjectProposal.pdf
└── assets/
    ├── characters/
    ├── maps/
    └── UI/
```

⚠️ Source code and assets stored in Google Drive (not public on GitHub).

## 💻 Minimum System Requirements

These are the recommended system specifications for playing or testing the game (non-optimized performance assumed):

| Component | Minimum Requirement |
| --- | --- |
| OS | Windows 10 (64-bit) |
| CPU | Intel Core i5-7400 / AMD Ryzen 5 1400 |
| RAM | 8 GB |
| GPU | NVIDIA GTX 1050 Ti / AMD RX 560 (2-4 GB VRAM) |
| Storage | At least 20 GB free (for Unreal + assets) |
| Disk Type | SSD (preferred) or 7200 RPM HDD |
| DirectX | Version 12 |
| Engine Version | Unreal Engine 5.6 |

**Development Machine**: Core i5 or Ryzen 5, 8–16 GB RAM, SSD, GTX 1050 or above

⚠️ Lower-end PCs may experience stutters. No ray tracing or ultra graphics used.

## 🔐 Security & Backups

- Code versioning and backups via GitHub (for docs) and Google Drive (for source/assets)
- Weekly local backups and manual snapshots during major changes
- Critical assets tracked with source versioning

## 👥 Team Roles (Technical)

| Name | Role | Responsibility |
| --- | --- | --- |
| Affan | C++ Dev, Core Mechanics | Player logic, AI shooting, DSA code, UI connections |
| Umar | Blueprints + Assets | Map setup, imported characters, Blueprint prototyping |

## 📌 Final Notes

- **Scope**: 1 Map, 1 Mission, 4-player squad (1 player + 3 AI), core features only
- **Delivery**: GitHub (docs), Google Drive (project files), Demo Video
- **Timeline**: 8 weeks from setup to polish (Jul 5–Aug 29, 2025)