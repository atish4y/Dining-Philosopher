
# 🍽️ Dining Philosophers Problem — Monitor-Based Visualization

An **interactive web-based simulation** that visualizes the **Dining Philosophers Problem** using the **Monitor synchronization concept** from Operating Systems.  
Built entirely with **HTML, CSS, and JavaScript**, this tool demonstrates how philosophers think, eat, and share chopsticks in a deadlock-free environment.

---

## 🎯 Overview

This project graphically represents **five philosophers** sitting around a circular table.  
Each philosopher alternates between **thinking**, **getting hungry**, and **eating**, while ensuring no two adjacent philosophers eat simultaneously — maintaining mutual exclusion and avoiding deadlock.

It’s an ideal project for understanding and visualizing the **Monitor-based synchronization solution** to one of the most classic OS concurrency problems.

---

## 🧠 Core Concepts

- **Monitor Synchronization:**  
  Manages shared resources (chopsticks) safely between concurrent processes (philosophers).

- **Philosopher States:**  
  - 🟠 **Thinking** — philosopher is not using chopsticks  
  - 🟡 **Hungry** — waiting to acquire both chopsticks  
  - 🔵 **Eating** — currently eating (both chopsticks held)

- **Chopstick States:**  
  - ⚫ **Available** — free to use  
  - 🔵 **In Use** — currently held by a philosopher  

---

## ⚙️ Features

✅ Interactive **Start**, **Reset**, **Step Forward**, and **Step Backward** controls  
✅ Adjustable **Think Time** and **Eat Time** parameters  
✅ Real-time **status updates** (current step, total steps, simulation state)  
✅ Dynamic **execution log** for understanding each action  
✅ Visually appealing dark UI with color-coded elements  
✅ 100% client-side — no frameworks or backend needed  

---

## 🧩 Technologies Used

- **HTML5** — Structure and layout  
- **CSS3** — Styling and responsive design  
- **JavaScript (ES6)** — Logic, simulation, and rendering  
- **Canvas API** — For drawing philosophers and chopsticks  

---

## 🚀 How to Run

1. **Clone the Repository**
   ```bash
   git clone https://github.com/atish4y/dining-philosopher.git
Navigate to the Project Folder

bash
Copy code
cd dining-philosopher
Open the HTML File

bash
Copy code
open index.html
(or simply double-click the file to open in your browser)

🧮 Simulation Flow
Step	Action	Description
0	Initial State	All philosophers are thinking
1	P0 picks up chopsticks	P0 starts eating
2	P2 picks up chopsticks	P2 starts eating
3	P4 picks up chopsticks	P4 starts eating
…	...	...
n	Philosopher puts down chopsticks	Chopsticks become available

You can move forward/backward step-by-step to observe how the monitor ensures fairness and avoids deadlock.

🎨 UI Overview
Canvas Section: Displays philosophers and chopsticks

Control Panel: Allows running and managing the simulation

Legend Section: Explains color codes for states

Execution Log: Lists chronological steps of the simulation
