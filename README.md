# AI-Agent-based-Solution
Artificial Intelligence Search Algorithms Implementation  

## Overview  
This repository contains implementations of **AI search algorithms** applied to **real-world problem scenarios**, including **Room Service Robot** and **Bridge Crossing Problem**. The solutions utilize **Depth-First Search (DFS), Iterative Deepening Depth-First Search (IDDFS), and Uniform Cost Search (UCS)** to find optimal paths while satisfying given constraints.  

## Table of Contents  
- [Room Service Robot](#room-service-robot)  
- [Bridge Crossing Problem](#bridge-crossing-problem)  
- [Technologies Used](#technologies-used)  
- [How to Run](#how-to-run)  
- [Example Inputs & Outputs](#example-inputs--outputs)  
- [License](#license)  

---

## Room Service Robot  
### 📌 Problem Statement  
A **Room Service Robot** must serve **three rooms (A, B, C)** while **minimizing the movement cost**. The robot must return to the **Service Room** after serving each room.  

### 🔹 **Algorithm Used**  
- **Depth-First Search (DFS)** – Explores paths deeply before backtracking.  
- **Iterative Deepening Depth-First Search (IDDFS)** – Combines DFS and BFS for efficient depth exploration.  

### 🔹 **Constraints**  
- The robot starts at the **Service Room**.  
- It must **serve each room exactly once** before stopping.  
- After serving a room, it **must return to the Service Room** before serving another.  
- Movement costs vary based on direction:  
  - Left Move + Serve: **5**  
  - Right Move + Serve: **5**  
  - Up Move + Serve: **1**  
  - Returning to Service Room: **0**  

### 🔹 **Expected Output (Example)**  
```txt
DFS Path: Service Room → Room A → Service Room → Room B → Service Room → Room C → Service Room  
DFS Total Cost: 16  
IDDFS Path: Service Room → Room C → Service Room → Room A → Service Room → Room B → Service Room  
IDDFS Total Cost: 11

