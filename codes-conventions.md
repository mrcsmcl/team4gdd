---
title: Technical Codes and Conventions
description: 
published: 1
date: 2025-01-14T15:33:13.056Z
tags: 
editor: markdown
dateCreated: 2025-01-14T15:33:13.056Z
---

# Unreal Engine File Organization

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


# GitHub Organization: GitFlow Workflow

To improve how we manage our work on GitHub, we will adopt the GitFlow workflow. This structured branching strategy will help maintain an organized repository, reduce conflicts, and ensure clarity in project contributions. Below is a detailed explanation of the workflow:

## Key Branches

GitFlow defines two main persistent branches in the repository:

1. **Main/Master Branch**:
   - This branch contains the stable, release-ready version of the project.
   - Only thoroughly tested and approved changes are merged into this branch.
   - It represents the production-ready state of the application.

2. **Development Branch**:
   - The primary working branch where ongoing development occurs.
   - All feature, bugfix, or hotfix branches are merged into this branch after thorough testing.
   - Represents the integration state of the project, which may include work-in-progress changes.

<br>

## Feature Branch Workflow

When contributing to the project, follow these steps to maintain a clean and organized repository:

<br>

### 1. **Create a Feature Branch**
   - Always start by creating a new branch from the `Development` branch.
   - Use a clear and descriptive naming convention to indicate the purpose of the branch. Examples:
     - `feature/ai-movement` for new AI movement functionality.
     - `bugfix/collision-detection` for fixing a collision detection issue.
     - `hotfix/ui-bug` for urgent fixes to production bugs.

<br>

### 2. **Work on the Feature**
   - Commit your changes regularly with clear and concise commit messages.
   - Test your changes locally to ensure they do not introduce new issues.

<br>

### 3. **Merge Back into Development**
   - Once your feature or fix is complete, create a pull request (PR) to merge the branch into `Development`.
   - Review and resolve any merge conflicts.
   - Ensure all automated tests pass, and get the PR reviewed by a teammate if possible.


<br>

### 4. **Delete the Branch**
   - After successfully merging the branch, delete it from the repository.
   - This step prevents clutter and ensures that only active branches remain visible.
   - If the code needs to be revisited, the commit history retains all previous changes.

<br>

## Why Deleting Branches is Important

Deleting branches after merging is recommended for the following reasons:
- **Reduces Clutter**: Keeps the repository clean and easy to navigate.
- **Ensures Focus**: Highlights only active and relevant branches for the team.
- **Commit History as a Record**: If old code needs to be revisited, the full history is available in the repository.

<br>
--

By adopting this workflow, we achieve several benefits: contributions are organized, as everyone knows where to begin their work and how to integrate it back into the project; conflicts are reduced through a clear separation of concerns, which minimizes merge issues; releases become more efficient, as stable versions can be created from the `Main/Master` branch without interrupting ongoing development; and collaboration is improved, thanks to a well-defined structure that enables team members to work independently without confusion.
