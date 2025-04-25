# ✈️ Decentralized Deep Reinforcement Learning for Dynamic Flight Path Recalibration in Weather and Traffic Conditions

This repository contains the source code, Jupyter Notebook, and supporting files for the Capstone project titled:

---

This project presents a decentralized approach to optimizing aircraft flight paths by integrating **real-time weather** and **air traffic data** using **Deep Reinforcement Learning (DRL)**. A hybrid optimization engine combining reinforcement learning with traditional algorithms dynamically generates optimal, weather-diverted, and traffic-avoidance paths.

Key Outcomes:
- 95% path similarity to shortest paths
- 97% route efficiency
- Navigation precision with average error of 11.7 km
- 12% and 14% efficiency impact for weather and traffic, respectively

---

## 🧠 Core Concepts

- **Adaptive Network Graph**: Incorporates real-time NOAA (weather) and ADS-B Exchange (traffic) data.
- **Composite Edge Weights**: Weighted by distance, weather severity, and traffic congestion.
- **Dueling Deep Q-Network (DDQN)**: Used for learning dynamic flight policies.
- **Multi-Objective Optimization**: Generates paths based on prioritized parameters (distance, safety, fuel).

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/flight-path-optimization.git
cd flight-path-optimization
```
### 2. Create a virtual environment (optional but recommended)
```
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```
---
### 🚀 How to Run
### 1. Launch Jupyter:
```
jupyter notebook
```
2.Open `Flight path recalibration.ipynb`

3.Run the notebook step by step to explore the architecture, data processing, model training, and results.

---
### 📊 Data Sources
Weather Data: NOAA API (15-min interval updates)

Traffic Data: ADS-B Exchange (real-time aircraft positioning)

---

## 📍 Evaluated Routes

| Route                                  | Region |
|----------------------------------------|--------|
| Delhi (VIDP) → Chennai (VOMM)          | India  |
| Mumbai (VABB) → Delhi (VIDP)           | India  |
| New York (KJFK) → Los Angeles (KLAX)   | USA    |
| London (EGLL) → Frankfurt (EDDF)       | Europe |

---

## 📈 Results Summary

| Metric                        | Value    |
|------------------------------|----------|
| Optimal Path Similarity      | 95%      |
| Route Efficiency             | 97%      |
| Weather Impact on Efficiency | 12%      |
| Traffic Impact on Efficiency | 14%      |
| Mean Navigation Error        | 11.7 km  |
