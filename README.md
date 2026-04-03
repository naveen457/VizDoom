# 🚀 Efficient PPO Training in VizDoom using Model Checkpointing

This project implements a **Proximal Policy Optimization (PPO)** based Reinforcement Learning agent in the **VizDoom environment**, enhanced with **model checkpointing** to improve training efficiency.

---

## 📌 Project Overview

Reinforcement Learning (RL) enables agents to learn optimal actions through interaction with an environment. However, training RL models from scratch is computationally expensive, especially in complex environments like **VizDoom**.

This project introduces a **checkpoint-based training approach**, allowing models to:
- Save progress during training
- Resume training from saved states
- Avoid redundant computation

---

## 🎯 Objectives

- Implement PPO-based RL agent in VizDoom  
- Integrate checkpointing for continuous training  
- Compare **scratch training vs checkpoint training**  
- Improve convergence speed and training efficiency  

---

## 🧠 Key Concepts

### 🔹 PPO (Proximal Policy Optimization)
- Policy gradient method  
- Uses **Actor-Critic architecture**  
- Provides stable and efficient learning  

### 🔹 Checkpointing
- Saves model weights periodically  
- Allows training to resume  
- Reduces retraining time  

---

## 🏗️ System Workflow

1. Initialize VizDoom environment  
2. Select scenario (Basic / Defend the Center)  
3. Train PPO agent  
4. Save model checkpoints  
5. Reload model  
6. Continue training  

---

## 📊 Results Summary

| Metric              | From Scratch | With Checkpoint |
|--------------------|-------------|-----------------|
| Training Time      | High        | Reduced         |
| Convergence Speed  | Slow        | Faster          |
| Efficiency         | Low         | High            |

### 🔥 Key Insight:
> Checkpoint-based training achieves faster convergence and reduces training time while maintaining performance.

---

## 📈 Graphs

### 🔹 Learning Curve
![Learning Curve](images/rewardvsmean.png)

### 🔹 Checkpoint vs Scratch Comparison
![Comparison](images/EpisodeRewardMeanvsTimeStamps.png)

---

## 🧪 Validation

The system was validated using two VizDoom scenarios:

### ✅ Basic Scenario
- Faster convergence  
- Stable reward growth  
- Lower complexity  

### ⚠️ Defend the Center
- Slower convergence  
- Higher complexity  
- More dynamic environment  

### 📌 Observations
- Increased complexity → slower learning  
- PPO provides stable training  
- Checkpointing improves efficiency and continuity  

---

## ⚙️ Technologies Used

- Python  
- Stable-Baselines3  
- VizDoom  
- OpenAI Gym  
- PyTorch  

---

## ▶️ How to Run (Jupyter Notebook)

### 🔹 Step 1: Create Virtual Environment

```bash
# Create environment
python -m venv rl_env

# Activate environment (Windows)
rl_env\Scripts\activate

# Activate environment (Linux/Mac)
source rl_env/bin/activate
#install dependencies
pip install -r requirements.txt
