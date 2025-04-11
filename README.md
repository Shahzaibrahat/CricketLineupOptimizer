# CricketLineupOptimizer
Optimize cricket batting lineups using KDE and linear programming. Simulates player performance by location, applies constraints like run rate and position eligibility, and uses the Simplex method to maximize expected runs. Includes sensitivity analysis for flexibility impact.


# Optimal Cricket Batting Lineup Using Simulation & Optimization

This project explores how data science can be used to **optimize cricket batting lineups** based on location-specific performance data. By combining **Kernel Density Estimation (KDE)**, **Monte Carlo simulations**, and **Linear Programming**, we determine the most effective batting order for top Indian batsmen under realistic constraints.

##  Problem Statement

Determine the optimal batting order for the following players based on match location:

- **KL Rahul**
- **Virat Kohli**
- **Rishabh Pant**

Using performance data since 2015, the goal is to **maximize total expected runs** when playing in:

-  **India**
-  **England**

## Methodology

### Data Simulation
- Used **Kernel Density Estimation (KDE)** to simulate each player's runs, balls faced, and strike rate.
- Preserved realistic correlations using **Monte Carlo Simulation** by generating over multiple overs and scores.

### Optimization
- Formulated the problem as a **Linear Programming (LP)** task.
- Solved using the **Simplex method with Gurobi**.
- Key constraint: Players must have an **expected run rate > 0.6** in the assigned position for a specific location.

##  Results

### 🇮🇳 Stadium Location: **India**
- **KL Rahul** → Batting Position **4**  
- **Rishabh Pant** → Batting Position **5**  
- **Virat Kohli** → Batting Position **3**

### 🏴 Stadium Location: **England**
- **KL Rahul** → Batting Position **1**  
- **Rishabh Pant** → Batting Position **4**  
- **Virat Kohli** → Batting Position **3**


## Project Files

- `Jupyter_file.ipynb` — Full code for data processing, simulation, and optimization  
- `Report.pdf` — Project summary and results  
- `References.docx` — Resources and citations  
- `README.md` — Project overview


## Future Scope

- Extend the model to full team lineups  
- Include bowling data and opposition analysis  
- Add weather and pitch condition factors


## Let's Connect

Have feedback or ideas to improve the model? Feel free to fork, star, or reach out!

