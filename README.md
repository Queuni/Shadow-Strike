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

- Handle the duplicate key case by merging the values instead of failing

- Bump version to 1.2.0 and add changelog entry for the new features

- Simplify the auth flow by using a single token source

- Handle the partial write case and retry the remaining bytes

- Fix the memory leak in the long-running worker process

- Remove redundant check that was already covered by the validator

- Implement retry logic for the API client when the remote returns 5xx

- Clean up debug print statements before the release

- Handle the partial write case and retry the remaining bytes

- Correct the docstring to match the actual behavior of the function

- Clean up debug print statements before the release

- Improve test coverage for the helpers module to above 90%

- Correct the default value for the feature flag in production

- Support passing options through the config file as well as CLI
