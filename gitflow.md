---
title: GitHub Organization
description: 
published: 1
date: 2025-01-15T21:37:53.470Z
tags: organization, gitflow, github
editor: markdown
dateCreated: 2025-01-14T15:36:59.123Z
---

# GitFlow Workflow

To improve how we manage our work on GitHub, we will adopt the GitFlow workflow. This structured branching strategy will help maintain an organized repository, reduce conflicts, and ensure clarity in project contributions. Below is a detailed explanation of the workflow:

<br>

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

By adopting this workflow, we achieve several benefits: contributions are organized, as everyone knows where to begin their work and how to integrate it back into the project; conflicts are reduced through a clear separation of concerns, which minimizes merge issues; releases become more efficient, as stable versions can be created from the `Main/Master` branch without interrupting ongoing development; and collaboration is improved, thanks to a well-defined structure that enables team members to work independently without confusion.
