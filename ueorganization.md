---
title: Unreal Engine File Organization
description: 
published: 1
date: 2025-02-13T23:39:07.685Z
tags: file, organization, unreal engine
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

Maintaining clear and consistent naming conventions is essential for effective project organization and collaboration. By following these conventions, team members can easily understand the content of a file just by looking at its name, which reduces confusion and enhances workflow efficiency. Below are more detailed examples for each type of asset:

<br>

### **Blueprints**:  
Blueprint naming should reflect the role or functionality of the object or system being designed. For example:
- `BP_Character_Player`: This indicates a Blueprint for a playable character within the game.
- `BP_Enemy_AI`: Represents a Blueprint for non-playable characters (NPCs) with artificial intelligence.

<br>

### **Textures**:  
Textures are often categorized based on their use in the game, such as environment, characters, or materials. Examples:
- `T_Wood_01`: This texture represents a wooden material. It includes a prefix `T_` indicating that it is a texture, followed by the material type (`Wood`) and a number (`01`) to differentiate multiple variations or versions.
- `T_Metal_02`: Similarly, this texture is a metallic material, with the numbering allowing for multiple versions or specific variations to be easily distinguished.

<br>

### **Static Meshes**:  
Static meshes are 3D models that do not animate. Naming conventions for these assets include:
- `SM_Tree_01`: Represents a tree static mesh, where `SM_` stands for Static Mesh, followed by the asset type (`Tree`) and a version number (`01`).
- `SM_Building_02`: A building model, where `SM_` denotes a static mesh, `Building` indicates the type, and `02` is the version identifier for different models or variations of buildings.

<br>

This standardization allows quick identification of specific static meshes within the project's assets, which is crucial for consistent use throughout different scenes or levels. By adhering to these naming conventions, team members can easily search, categorize, and maintain assets within the Unreal Engine project, promoting better collaboration and project management.

<br>

## 3. Personal Working Folders

<br>

Team members actively working on specific tasks should create personal folders under `Development`. Each folder should be named after the individual (e.g., `Development/John`). Once the work is completed and tested, files should be moved into the appropriate root folder.

<br>

## 4. Regular Cleanup and Maintenance

At the conclusion of each team meeting, we will collectively review the file organization. This review will ensure that assets are correctly placed, unused or temporary files are removed, and the overall structure remains clean and functional.