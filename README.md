# 🔧 An Autonomous Traffic Light Control System Using Q-Learning

This project simulates an intelligent traffic light control system using **Q-learning**, a type of **reinforcement learning**, to minimize vehicle congestion at a 4-way intersection.

### 🔍 Problem Statement

Traffic congestion is a critical issue in urban environments. Conventional traffic lights work on fixed timers and cannot adapt to real-time traffic flow. In this project, I build a **self-learning agent** that dynamically decides which direction gets a green signal based on traffic queue lengths at each direction (North, East, South, West).

---

### 🧠 Solution Overview

I implement a custom **Q-learning agent** that learns to:

- Observe traffic queue lengths (state)
- Choose the best traffic light action (green for N-S, E-W, or all-red)
- Receive rewards (shorter queues = better reward)
- Learn over time to reduce overall congestion

---

### ⚙️ How It Works

- The environment simulates random vehicle arrivals at each direction.
- Actions:
  - `0`: Green for North-South
  - `1`: Green for East-West
  - `2`: All-red (for emergency pause or cooldown)
- The Q-learning agent discretizes states and updates its policy based on received rewards.
- The learning loop runs over multiple episodes until the agent improves decision-making.

---

### 📊 Visualization

I animate the simulation using `matplotlib.animation`:

- Bars represent queue lengths for each direction.
- Green bars = lanes allowed to move (green light).
- Red bars = lanes stopped (red light).
- Real-time updates show how the agent adapts to traffic conditions.

---

### 📁 Files

- `traffic_q_learning.py` — core environment and agent code
- `traffic_simulation.ipynb` — interactive notebook with code, training, and visualization
- `README.md` — project overview

---

### 🚀 Technologies Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

---

### ✅ Future Enhancements

- Add real-world data integration (e.g., vehicle sensors)
- Use Deep Q-Learning (DQN) for more complex intersections
- Support multi-agent intersections

---

### 👤 Author

**Enkeshie Parris**\
*Machine Learning Analyst / Data Scientist*\
Feel free to connect with me on [LinkedIn](#) or explore more of my work!

