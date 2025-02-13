---
title: Characters and AI
description: 
published: 1
date: 2025-02-13T23:38:11.759Z
tags: ai, characters
editor: markdown
dateCreated: 2024-10-24T13:21:29.347Z
---

# Characters and AI Design

This section delves into the mechanical attributes of the game's characters, as well as the design of NPCs and their AI behaviors.

---

## **Main Characters**

### **Leo**  
**Gameplay Role**  
- Primary focus on stealth mechanics and physical interaction with the environment.  
- Can crouch, climb, vault over obstacles, and use cover to avoid detection.  
- Equipped with basic tools like a lockpick, throwable distractions (e.g., coins), and a stun device for incapacitating guards.  

**Animations**  
- Fluid, parkour-inspired movements for climbing and sneaking.  
- Tense idle animations when hiding or observing enemies.  
- Quick and reactive animations during chases or combat scenarios.  

---

### **Vinny**  
**Gameplay Role**  
- Operates as the team's hacker, controlling the game's 2D interface.  
- Accesses cameras, unlocks doors, disables alarms, and gathers intel on enemy positions.  
- Provides critical support to Leo via real-time communication and problem-solving.  

**Animations**  
- Limited to sitting or standing at the virtual computer station.  
- Subtle movements, like typing, leaning forward, or adjusting his glasses, emphasize his focus on the task.  

---

## **Non-Playable Characters (NPCs)**

### **Security Guards**  
**Physical Description**  
- Varied physiques, but all wear professional high-tech uniforms, including helmets and visors with integrated HUDs.  
- Their gear includes utility belts, flashlights, and tasers.  

**AI Behavior**  
- Patrol set paths but can dynamically adjust based on player actions (e.g., noises, footprints, or suspicious objects).  
- Collaborative behavior when investigating, with guards calling for backup or spreading out to search.  
- Alert states:  
  - **Normal:** Patrolling.  
  - **Suspicious:** Investigating noise or movement.  
  - **Alert:** Actively pursuing Leo.  

**Animations**  
- Realistic walking and searching motions.  
- Reactive animations for spotting the player, using communication devices, or drawing weapons.  

---

### **Neotech Employees**  
**Physical Description**  
- Formal attire that reflects their roles, from lab coats to suits.  
- Some may carry personal items like ID badges, tablets, or coffee mugs.  

**AI Behavior**  
- Passive NPCs who react to unusual activity but are not actively hostile.  
- May alert guards if they notice suspicious activity.  

**Animations**  
- Idle behaviors like typing, talking, or walking between rooms.  

---

## **Environment-Specific NPCs**

### **Café Customers**  
- Relaxed attire, reflecting a casual atmosphere.  
- Idle animations include sipping coffee, chatting, or reading.  

### **Warehouse Workers**  
- Work uniforms with protective gear like gloves and helmets.  
- Perform routine tasks like moving crates or operating forklifts.  

### **Neotech Specialists**  
- Appear in high-security zones with more advanced attire, including lab coats or augmented reality glasses.  
- Engage in technical tasks or monitor security systems.

---

## **AI Behavior Design**

### **Awareness System**  
- AI reacts to sound, line-of-sight, and environmental triggers.  
- Guards have cone-shaped vision fields that can be altered based on environmental lighting.  

### **Cooperation**  
- Guards work together, communicating via radios to strategize and flank the player.  
- In high-security areas, guards may deploy drones or other automated systems.  

---

## **Character and AI Animation Techniques**

### **Blending and Layering**  
- Smooth transitions between stealth, idle, and action animations for fluid gameplay.  

### **Dynamic Reactions**  
- Contextual animations, such as a guard checking a noise or reacting to a disabled camera.  

### **Attention to Detail**  
- Subtle environmental interactions, such as a guard leaning on a desk or an NPC checking their watch, to make the world feel alive.  