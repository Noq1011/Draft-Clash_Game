# Draft Clash (Prototype)

## Overview
Draft Clash is a prototype for a 2D multiplayer auto-battler that combines budget-based drafting mechanics with arcade-style combat. 

This repository contains the core game logic, including the auto-battler initiative queue, UI health management, and the drafting phase manager.

## Architecture & Systems
* **Drafting Phase Manager:** A 60-second blind-bidding system where players allocate a set budget to draft characters from a shared pool.
* **Auto-Battler Combat Logic:** A custom C# initiative and attack queue that calculates damage, applies archetype modifiers, and triggers floating UI text.
* **Backend Database Schema:** PostgreSQL and Redis schemas designed to manage player Elo, inventory unlocks, and persistent cross-session data.
* **Character Data Structures:** Unity `ScriptableObjects` managing 15 distinct archetype stats and behavioral tags.

## Tech Stack
* **Language:** C#
* **Databases:** PostgreSQL, Redis
* **Game Engine Concepts:** ScriptableObjects, Coroutines, UI Canvas management, Event-driven architecture.
