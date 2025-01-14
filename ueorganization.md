---
title: Unreal Engine File Organization
description: 
published: 1
date: 2025-01-14T15:40:16.365Z
tags: 
editor: markdown
dateCreated: 2025-01-14T15:33:13.056Z
---

# File Organization

To ensure a smooth workflow and minimize confusion when multiple team members are working in Unreal Engine, it is essential to implement a structured and well-documented file organization system. This organization will make it easier for everyone to locate and save assets while reducing the likelihood of conflicts, redundant work, and misplaced files. Below is a detailed explanation of the proposed system:

## 1. Root Folder Structure

All files within the `Content` folder will be categorized into clearly defined root folders based on their type or purpose. Each root folder will contain subfolders for further classification. The structure is as follows:

- **Art**:
  - `Art/Textures`: Contains all texture files, organized further by type:
    - `Textures/Environment`: Environment-related textures.
    - `Textures/Characters`: Character textures.
  - `Art/Materials`: Includes materials and material instances.
  - `Art/UI`: Stores all visual assets related to the user interface.

- **Blueprints**:
  - `Blueprints/Characters`: Blueprints for both playable characters and NPCs.
  - `Blueprints/Gameplay`: Core game mechanic Blueprints, such as pickups or interactables.
  - `Blueprints/UI`: Blueprints related to user interface logic and widgets.

- **Meshes**:
  - `Meshes/Characters`: Models for characters.
  - `Meshes/Environment`: Assets for environmental elements, such as trees, buildings, and props.
  - `Meshes/Weapons`: Models for weapons or tools.

- **Animations**:
  - `Animations/Characters`: Animation sequences and related Blueprints for characters.
  - `Animations/Props`: Animations for props and other environmental interactions.

- **Audio**:
  - `Audio/SFX`: Sound effects for the game.
  - `Audio/Music`: Background music files.
  - `Audio/Voice`: Audio files for voiceovers or character dialogue.

- **Levels**:
  - `Levels/Main`: Main game levels used in production.
  - `Levels/Test`: Maps and levels for testing or prototypes.

- **UI**:
  - `UI/Widgets`: Widget Blueprints for HUDs, menus, and other interface elements.
  - `UI/Textures`: UI-specific textures, such as icons and buttons.

<br>

## 2. Naming Conventions

To maintain clarity and consistency, all files should adhere to strict naming conventions. Examples include:

- **Blueprints**: `BP_Character_Player`, `BP_Enemy_AI`.
- **Textures**: `T_Wood_01`, `T_Metal_02`.
- **Static Meshes**: `SM_Tree_01`, `SM_Building_02`.

<br>

## 3. Personal Working Folders

<br>

Team members actively working on specific tasks should create personal folders under `Development`. Each folder should be named after the individual (e.g., `Development/John`). Once the work is completed and tested, files should be moved into the appropriate root folder.

<br>

## 4. Regular Cleanup and Maintenance

At the conclusion of each team meeting, we will collectively review the file organization. This review will ensure that assets are correctly placed, unused or temporary files are removed, and the overall structure remains clean and functional.