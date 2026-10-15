# BioSched — Smart Electricity Load Scheduling

**Bio-Inspired Computing Hackathon Project**

## 📌 Project Overview

BioSched is a smart electricity scheduling system that allocates household appliances to suitable operating periods to minimize electricity costs while satisfying user-defined operating constraints.

Electricity prices can vary throughout the day. BioSched uses bio-inspired optimization algorithms to find suitable appliance schedules that reduce estimated electricity expenses while respecting operating time windows and the maximum household load.

## 🎯 Objectives

- Minimize total household electricity cost.
- Schedule appliances within their allowed operating periods.
- Respect appliance operating durations and power constraints.
- Compare different bio-inspired optimization algorithms.
- Demonstrate Artificial Neural Networks and supervised, unsupervised, and reinforcement learning.
- Visualize appliance schedules, electricity costs, and household load.

## 🧠 Algorithms and Technologies

| Technique | Application |
|---|---|
| Hill Climbing | Improves a schedule through local search. |
| Simulated Annealing | Explores alternative schedules and helps escape local optima. |
| Genetic Algorithm | Optimizes schedules using selection, crossover, mutation, and elitism. |
| Artificial Neural Network (ANN) | Demonstrates electricity-price pattern prediction. |
| Supervised Learning | Trains a neural network using example price data. |
| Unsupervised Learning | Uses K-Means to group hours by electricity-price patterns. |
| Reinforcement Learning | Demonstrates Q-learning for appliance start-time selection. |

## ⚙️ How It Works

1. Define household appliances, their power consumption, operating durations, and allowed start times.
2. Provide hourly electricity prices.
3. Calculate the estimated electricity cost of each schedule.
4. Apply bio-inspired algorithms to search for lower-cost schedules.
5. Check scheduling constraints and maximum combined household load.
6. Compare algorithm performance and visualize the results.

## 📐 Cost Function

The estimated electricity cost is calculated as:

**Total Cost = Sum of (Appliance Power × Hourly Electricity Price)**

This calculation is performed for every hour that an appliance operates.

Schedules that violate configured constraints receive penalties during optimization. The final feasibility check verifies legal start times, operating durations, and the maximum combined load.

## 📊 Visualizations

The Google Colab notebook includes:

- Hourly electricity-price graph.
- Baseline schedule and cost calculation.
- Hill Climbing convergence graph.
- Simulated Annealing convergence graph.
- Genetic Algorithm convergence graph.
- Algorithm comparison table.
- Appliance scheduling Gantt chart.
- Hourly household load profile.
- ANN price-prediction visualization.
- K-Means price-clustering visualization.
- Q-learning demonstration.
- Final cost and feasibility summary.

## 🛠️ Technologies Used

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## 🚀 How to Run the Project

### Using Google Colab

1. Download `BioSched_Human_Readable_Colab.ipynb` from the project files.
2. Open [Google Colab](https://colab.research.google.com/).
3. Select **File → Upload notebook**.
4. Upload the notebook.
5. Select **Runtime → Run all**.
6. Review the generated schedules, graphs, comparison tables, and final results.

### Running Locally

Install Python 3.10 or later and the required libraries:

```bash
pip install numpy pandas matplotlib scikit-learn
```

Open the notebook using Jupyter Notebook or JupyterLab and execute the cells sequentially.

## 📁 Repository Structure

```text
BioSched-Smart-Electricity-Load-Scheduling/
├── README.md
├── BioSched_Human_Readable_Colab.ipynb
```

## 🏆 Expected Outcomes

The project compares optimization algorithms based on estimated electricity cost, objective score, and schedule feasibility.

The final output provides an appliance timetable, total estimated electricity cost, potential savings against a baseline schedule, and the peak combined household load.

Actual results depend on the tariff data, appliance configurations, constraints, and algorithm parameters.

## ⚠️ Limitations

- The included electricity prices are illustrative and are not live utility tariffs.
- ANN training uses synthetic example data for demonstration.
- The current implementation focuses on a single-day scheduling horizon.
- Optimization results depend on algorithm settings and search quality.

## 🔮 Future Enhancements

- Integrate real electricity tariffs and historical consumption data.
- Add an interactive interface for household preferences.
- Include appliance deadlines and user-defined priorities.
- Integrate solar panels and battery storage.
- Connect smart meters for real-time monitoring.
- Improve feasibility guarantees using constraint-aware optimization.



Replace these role descriptions with the actual names and contributions of your team members before submission.

## 📚 Conclusion

BioSched demonstrates how bio-inspired computing techniques can be applied to household electricity scheduling. By combining optimization algorithms, learning demonstrations, and visual analytics, the project explores ways to reduce estimated electricity costs while respecting household operating constraints.

**Project:** BioSched — Smart Electricity Load Scheduling  
**Platform:** Google Colab  
**Language:** Python
