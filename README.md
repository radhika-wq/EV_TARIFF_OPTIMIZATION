# 🚗 Agentic AI-Based Dynamic Tariff Optimization for EV Charging Networks

## 📌 Project Overview

The rapid adoption of Electric Vehicles (EVs) has created new challenges for charging infrastructure operators. Fixed electricity tariffs often lead to inefficient charger utilization, congestion during peak periods, and missed revenue opportunities.

This project develops an Agentic AI Framework for EV charging networks that combines:

- Demand Prediction Agent
- Dynamic Tariff Pricing Agent
- Monitoring & Learning Agent

The system analyzes charging behavior, predicts charging demand, adjusts tariffs dynamically, and evaluates operational performance using real-world EV charging datasets.

---

# 🎯 Objectives

The primary objectives of this project are:

- Forecast EV charging demand using machine learning
- Design a dynamic pricing mechanism based on demand levels
- Improve revenue generation compared to fixed tariffs
- Analyze charger utilization patterns
- Estimate off-peak charging uplift
- Monitor operational efficiency through performance metrics
- Demonstrate an Agentic AI workflow for smart charging networks

---

# 🧠 Agent Architecture

The project is divided into three intelligent agents:

## 1. Demand Prediction Agent

Responsible for forecasting charging demand using historical charging session information.

### Inputs

- Hour of day
- Weekend indicator
- Historical charging behavior
- Session characteristics

### Model Used

- Random Forest Regressor

### Output

Predicted charging demand (kWh)

---

## 2. Dynamic Tariff Pricing Agent

Adjusts charging tariffs according to predicted demand levels.

### Pricing Logic

| Demand Level | Tariff |
|-------------|---------|
| Low Demand | ₹10 / kWh |
| Medium Demand | ₹15 / kWh |
| High Demand | ₹25 / kWh |

### Goal

- Increase revenue
- Encourage off-peak charging
- Reduce charging congestion

---

## 3. Monitoring & Learning Agent

Evaluates system performance using operational metrics.

Tracks:

- Revenue Gain
- Pricing Efficiency
- Charger Utilization Rate
- Off-Peak Uplift
- Waiting Time Reduction (Proxy)
- Customer Response Rate

---

# 📊 Datasets Used

## Dataset 1: ACN Charging Dataset

Used for:

- Demand Forecasting
- Dynamic Tariff Pricing
- Revenue Analysis
- Pricing Efficiency Calculation

### Features

- Connection Time
- Disconnection Time
- Charging Completion Time
- Energy Delivered (kWh)
- Station Information

### Source

ACN Data Portal (Caltech EV Charging Network)

---

## Dataset 2: UrbanEV / ST-EVCDP Dataset

Used for:

- Charger Utilization Analysis
- Occupancy Analysis
- Charging Volume Analysis
- Off-Peak Uplift Estimation
- Monitoring Agent Metrics

### Dataset Statistics

- 24,798 charging piles
- Large-scale urban charging data
- Shenzhen, China
- 5-minute interval observations

### Source

https://github.com/IntelligentSystemsLab/ST-EVCDP

---

# 🔧 Project Workflow

```text
Raw Data
    ↓
Data Cleaning
    ↓
Feature Engineering
    ↓
Exploratory Data Analysis
    ↓
Demand Prediction Agent
    ↓
Dynamic Tariff Pricing Agent
    ↓
Monitoring & Learning Agent
    ↓
Performance Evaluation
```

---

# 📈 Feature Engineering

### ACN Dataset

- Session Duration (hours)
- Charging Duration (hours)
- Hour of Day
- Day of Week
- Weekend Indicator

### UrbanEV Dataset

- Average Occupancy
- Average Charging Volume
- Charger Utilization Rate
- Off-Peak Demand Statistics

---

# 🤖 Machine Learning Model

## Random Forest Regressor

The demand prediction model was trained using engineered charging features.

### Evaluation Results

| Metric | Value |
|----------|---------|
| MAE | 18.14 |
| RMSE | 37.31 |
| R² Score | 0.9595 |

### Interpretation

The model achieves a high R² score, indicating strong predictive capability for EV charging demand and making it suitable for dynamic pricing decisions.

---

# 💰 Revenue Optimization Results

## Fixed Tariff Revenue

₹203,628.40

## Dynamic Tariff Revenue

₹235,411.44

## Revenue Gain

**15.61%**

### Insight

Dynamic pricing generated significantly higher revenue compared to a fixed tariff strategy while maintaining operational efficiency.

---

# 📊 Monitoring Agent Metrics

| Metric | Value |
|----------|----------|
| Revenue Gain (%) | 15.61 |
| Pricing Efficiency | 17.34 |
| Charger Utilization Rate (%) | 69.49 |
| Off-Peak Uplift (%) | 34.40 |
| Waiting Time Reduction (%) | 25.60 |
| Customer Response Rate (%) | 13.33 |

---

# 📉 Key Insights

### Demand Prediction

- Charging demand exhibits strong hourly patterns.
- Peak charging activity occurs during specific periods of the day.

### Dynamic Pricing

- Revenue increased by over 15%.
- Demand-responsive pricing outperformed fixed tariffs.

### UrbanEV Analysis

- Average charger occupancy remains below maximum capacity.
- Significant opportunities exist for shifting demand toward off-peak periods.

### Monitoring Agent

- Improved utilization and operational efficiency.
- Demonstrated measurable benefits of AI-assisted charging management.

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- Jupyter Notebook
- GitHub

---

# 📂 Repository Structure

```text
EV_TARIFF_OPTIMIZATION
│
├── 01_json_to_csv.ipynb
├── 02_EDA.ipynb
├── 03_demand_prediction.ipynb
├── 04_monitoring_agent.ipynb
├── 05_STEVCDP_Analysis.ipynb
│
├── cleaned_acn_data.csv
├── occupancy.csv
├── volume.csv
├── stations.csv
│
├── demand_model.pkl
├── final_metrics_summary.csv
├── urbanev_occupancy_analysis.csv
│
└── README.md
```

---

# 🚀 Future Scope

- Reinforcement Learning-based tariff optimization
- Real-time EV charging demand forecasting
- Weather-aware charging demand prediction
- Grid load balancing integration
- Multi-city deployment of intelligent charging networks
- Smart charging recommendation systems

---

# 👩‍💻 Author

**Radhika (24117101)**  
B.Tech Mechanical Engineering  
Indian Institute of Technology Roorkee
