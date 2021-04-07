# Shadow Strike

A 3D stealth-action Unity game inspired by classic ninja titles. Built with clean architecture and scalability in mind.

---

## Overview

Control a nimble operative through hostile territory: sneak, strike, and use tools to complete objectives. The codebase is structured for maintainability and extension.

---

## Technical Highlights

| Area | Approach |
|------|----------|
| **Player** | FSM (finite state machine) for movement, combat, and stealth states |
| **AI** | Behaviour trees for patrol, search, and combat |
| **Weapons** | Inheritance-based system; items can act as melee, thrown, or ranged (e.g. sword that can be thrown, shuriken used in melee) |
| **Animation** | Single shared animator with layers, masks, behaviours, and overrides for multiple character types |
| **Spawn system** | Object pools + Scriptable Objects for configurable enemy waves |

Additional use of Unity IK rigging and HDRP (sky and volumetric fog).

---

## Gameplay

- **Movement:** Run, crouch, dodge, wall-lean to peek
- **Stealth:** Grappling hook, stealth takedowns
- **Combat:** Melee, thrown weapons, firearms; blocking and evasion
- **AI:** Enemies share similar capabilities and can search when they lose sight of the player
- **Physics:** Ragdoll reactions to explosions
- **Inventory:** Pick up and equip weapons during play

---

## Requirements

- **Unity** (compatible version per `ProjectSettings`)
- Open the project folder in Unity and use the built-in scene loader to run from the editor.

---

## Project Structure

- `Assets/Characters` — Player and enemy prefabs, AI, damage systems
- `Assets/WeaponSystem` — Melee, throwing, and firearm logic
- `Assets/!Tools` — Wave controller, weapon adder, sound manager
- `Assets/Scenes` — Game and menu scenes


- Adjust the default concurrency limit based on load test results
