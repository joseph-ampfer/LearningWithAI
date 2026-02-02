# Learning with AI - Joe Ampfer

## Overview

This repository documents my learning journey using AI assistance as part of my ASE 485 Capstone course. My capstone project, **Spell Arena**, is a Unity game that uses gesture recognition to cast spells with your hands. I am extending it to support **multiplayer gameplay**, which requires me to learn new networking concepts and technologies.

---

## Topic 1: Networking Fundamentals for Multiplayer Games

### Why I Need to Learn This

My capstone project is transitioning from a single-player experience to a multiplayer game. To successfully implement multiplayer functionality, I need to understand the foundational concepts of networked game development. Without this knowledge, I risk creating a game with poor synchronization, unfair gameplay due to authority issues, or a frustrating experience caused by latency and desync problems.

### What I Want to Learn

- **Client-Server Architecture**: Understanding the differences between client-hosted (listen servers) and dedicated server models, and which is appropriate for my game.
- **Authority and Ownership**: Learning which machine (server or client) should control specific game objects and actions to prevent cheating and ensure consistency.
- **State Synchronization**: How to keep game state consistent across all connected players, including player positions, spell effects, and game events.
- **Latency Compensation**: Techniques like client-side prediction, server reconciliation, and interpolation to make the game feel responsive despite network delays.
- **Network Topologies**: Understanding peer-to-peer vs client-server models and their trade-offs for real-time action games.

### How I Will Learn with AI

1. **Conceptual Q&A**: I will use AI to explain networking concepts in the context of real-time action games, asking for examples specific to gesture-based spell casting.
2. **Architecture Design**: I will discuss my game's requirements with AI to determine the best authority model (e.g., should spell casting be server-authoritative or client-authoritative with validation?).
3. **Problem Solving**: When I encounter synchronization issues during development, I will describe the problem to AI and work through potential solutions.
4. **Code Review**: I will have AI review my networking code to identify potential issues with authority, race conditions, or inefficient sync patterns.

---

## Topic 2: Unity Netcode for GameObjects

### Why I Need to Learn This

Unity Netcode for GameObjects is Unity's official networking solution for multiplayer games. Since Spell Arena is built in Unity, using Netcode for GameObjects will provide native integration with Unity's ecosystem, making implementation more straightforward than third-party solutions. Learning this specific framework is essential to implement the multiplayer features I need.

### What I Want to Learn

- **NetworkObject and NetworkBehaviour**: How to properly set up networked game objects and write networked scripts.
- **NetworkVariables**: Using synchronized variables to share state (e.g., player health, mana, active spell effects) across the network.
- **RPCs (Remote Procedure Calls)**: Implementing ServerRpc and ClientRpc to trigger actions across the network (e.g., casting a spell, taking damage).
- **Spawning and Despawning**: Managing networked object lifecycles for spells, projectiles, and player characters.
- **Ownership and Authority**: Configuring which client owns which objects and how authority transfers work in Netcode.
- **Connection Management**: Handling player connections, disconnections, and lobby/matchmaking integration.
- **Relay and Lobby Services**: Using Unity's Relay service to allow players to connect without port forwarding, and Lobby service for matchmaking.

### How I Will Learn with AI

1. **Implementation Guidance**: I will ask AI for step-by-step instructions on implementing specific Netcode features, such as "How do I synchronize gesture recognition results to the server?"
2. **Code Generation and Explanation**: I will use AI to help write NetworkBehaviour scripts and explain each component's purpose.
3. **Debugging Assistance**: When networking code doesn't behave as expected, I will share error messages and observed behavior with AI to diagnose issues.
4. **Best Practices**: I will ask AI about common pitfalls and best practices specific to Netcode for GameObjects, especially for fast-paced action games.
5. **Integration Questions**: I will work with AI to understand how to integrate Netcode with my existing gesture recognition system and spell casting mechanics.

---

## Learning Goals and Success Metrics

| Topic | Success Criteria |
|-------|------------------|
| Networking Fundamentals | I can explain client-server authority, implement lag compensation, and design a synchronization strategy for my game |
| Unity Netcode for GameObjects | I can implement a working multiplayer prototype where two players can connect, see each other, and cast spells that affect both clients |

---

## Repository Structure

```
/docs           - Notes and documentation from AI learning sessions
/examples       - Code examples and experiments
/screenshots    - Progress screenshots and diagrams
```

---

## Progress Log

*I will update this section as I learn and implement features.*

| Date | Topic | What I Learned | AI Tool Used |
|------|-------|----------------|--------------|
| | | | |

