# ⚡ Intelligent-Home-Energy-Management and EV Scheduling

## 🚀 Smart Scheduling of EVs Through Intelligent Home Energy Management Using Deep Reinforcement Learning

[![IEEE Paper](https://img.shields.io/badge/Paper-IEEE%20Access-blue.svg)](https://ieeexplore.ieee.org/abstract/document/10004664)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](./LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-yellow.svg)](https://www.python.org/)

---

## 🧾 Abstract

This article presents the deep reinforcement learning (DRL)-based smart scheduling in an intelligent home energy management system (SSIHEMS) for electric vehicles (EVs), utilizing rooftop photovoltaic (PV) generation. Optimizing home appliances to minimize consumption cost is challenging due to the randomness of electricity prices. The model-free DRL-based SSIHEMS aims to address this by managing home appliances and EV scheduling to reduce grid dependency.

Decisions include battery charging/discharging and EV scheduling using a collaborative approach. A custom gym environment feeds system states to the agent and receives a reward based on action selection. A case study validates the approach, showing effective scheduling with PV generation. Comparative analysis with traditional methods confirms the superiority of the DRL-based system.

### I have added comments in the code from chatgpt.

🔗 **[Read the Paper](https://ieeexplore.ieee.org/abstract/document/10004664)**

---

## 🎯 Objective

The system integrates energy storage (ES), home loads, and PVs to manage energy optimally. The goal is to reduce utility dependency by storing surplus renewable energy. With declining ES costs (now just a few hundred $/kWh), using clean energy has become viable for achieving zero carbon emissions.

The system manages common appliances—air conditioners, refrigerators, microwaves, and washing machines—using a data-driven DRL-based controller.

---

## 🧠 System Architecture

![🧠 System Block Diagram](Block_diagram.png)

---

## 🗃️ Appliances Used & Dataset

A large, open-source dataset from **Pecan Street Inc.** was used. It spans multiple years; a few weeks were selected for this case study. Appliances tracked include:

- Refrigerator
- Air Conditioner
- Dishwasher
- Washing Machine
- Microwave
- Lighting
- Clothes Dryer
- Overall House Load

Data points were recorded every 15 minutes for one year. Data wrangling was performed to extract technical characteristics of each appliance.

---

## 📊 Time Series Data Visualization

### Power Consumption Trends

![🧠 Time Series Visualization](DataVisualization.png)

### Appliance-Wise Dataset Mapping

![🧠 Dataset Appliances](Diagram.gif)

---

## 🔁 Sequential Decision Management

Reinforcement Learning (RL) is a sequential decision-making algorithm. The environment simulates energy decisions across a 24-hour period.

![🧠 RL Case Generalization](case_generalization.gif)

---

## 🔌 EV Scheduling at Profitable Times

The DRL agent schedules EV charging to minimize cost and utilize profitable electricity rate periods.

![🚗 EV Scheduling](Ev_Scheduling.png)

---

## ⚠️ Generalizability Across Scenarios

System behavior is tested against unseen power scenarios to assess the RL model’s generalization capabilities.

![⚡ Scenario Testing](Cases.gif)

---

## 💸 Profit-Oriented Energy Management

The agent learns to store energy when rates are low and sell or use it when rates are high—**without compromising user comfort**.

![💹 Profit Optimization](profit_gained.png)

---

## 📈 RL Agent Performance Metrics

Training progress is validated via reward and loss curves. A stable reward and low loss indicates successful learning, especially as stochastic noise trends to zero.

![📉 RL Agent Reward/Loss](RL_agent.png)

---


# 🛠️ Home Energy Management System (HEMS) with Deep Q-Learning Code Explaination
This project implements a Home Energy Management System (HEMS) that uses **Deep Q-Learning (DQN)** to optimize energy usage in a simulated environment. The system considers energy usage patterns, electric vehicle (EV) scheduling, and battery storage management in a home or microgrid setting.

## Overview

This repository contains code to train a **Deep Q-Network (DQN)** for decision-making in a **Home Energy Management System (HEMS)** simulation. The environment is built using a custom HEMS setup that includes a Markov Decision Process (MDP) model for energy management and decision-making.

### Key Components:
- **MDP_Development1.py**: Contains the implementation of the Markov Decision Process (MDP) that simulates energy management for a home or microgrid environment.
- **HEMS_Environment.py**: Defines the environment for the Home Energy Management System (HEMS), including energy consumption patterns, battery storage, and electric vehicle scheduling.
- **Conditional_Energy_Management.py**: Manages energy conditions and setups for the overall system.
- **Data_Handling.py**: Handles data preprocessing, such as reading and formatting the input data.
- **Modules.py**: Contains utility functions or additional modules required for the HEMS simulation.
- **DQN_Agent_training.py**: This script implements the training process for the Deep Q-Network (DQN) agent. It includes environment interaction, experience replay, epsilon-greedy action selection, and network updates.

## Setup

### Prerequisites

To run this project, you need to install the following dependencies:

```bash
pip install tensorflow gym numpy matplotlib

```


## 📚 Citation

@inproceedings{suleman2022smart,
  author    = {A. Suleman and M. A. Amin and M. Fatima and B. Asad and M. Menghwar and M. A. Hashmi},
  title     = {Smart Scheduling of EVs Through Intelligent Home Energy Management Using Deep Reinforcement Learning},
  booktitle = {2022 17th International Conference on Emerging Technologies (ICET)},
  location  = {Swabi, Pakistan},
  year      = {2022},
  pages     = {18--24},
  doi       = {10.1109/ICET56601.2022.10004664},
  keywords  = {Deep learning; Photovoltaic systems; Home appliances; Costs; Transportation; Reinforcement learning; Electric vehicles; Deep reinforcement learning; Home energy management; EV; demand response}
}

### 📬  Contact Ahmad Suleman engineersuleman118@gmail.com


