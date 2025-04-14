# Prep_view
# 🎯 Interview Agent PPO Fine-Tuning

This project fine-tunes a reinforcement learning agent using Proximal Policy Optimization (PPO) in a custom interview simulation environment.

## 🛠️ Features
- Checkpoint-based training
- Evaluation after each training chunk
- Custom reward tuning
- PPO via Stable-Baselines3

## 📁 Structure
- `InterviewEnv`: Custom environment
- `model_checkpoints/`: Saved models
- `logs/`: Evaluation logs

## 🚀 How to Run
Train and evaluate the PPO model chunk by chunk while saving checkpoints:
```python
model.learn(total_timesteps=chunk_size, callback=eval_callback)
