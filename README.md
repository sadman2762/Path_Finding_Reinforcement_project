# Pathfinding Ball with PPO in 3D Environments

This project demonstrates the implementation of **Proximal Policy Optimization (PPO)** for a reinforcement learning agent in a 3D environment. The agent, represented as a ball, learns to find the path to a target cube under various environmental setups. This work combines state-of-the-art RL techniques with engaging visual representations.

---

## Features

### 🌐 **3D Environment**
- A visually rich 3D space where the agent learns and navigates.
- Realistic physics-based interactions between the ball and its surroundings.

### ⚙️ **Parallel Environment Setup**
- Designed parallel training environments for increased efficiency.
- Used a "Solo" approach to independently handle multiple environments for robust training.

### 🛠️ **YAML Configuration**
- Modular and reusable YAML files for flexible configuration of training parameters.
- Facilitates experimentation and ensures reproducibility of results.

### 📊 **TensorBoard Integration**
- Integrated TensorBoard for monitoring training progress.
- Provides insights into reward curves, loss trends, and other vital statistics for fine-tuning.

### 🎨 **Dynamic Feedback System**
- Scripted intuitive visual feedback using Unity materials and C#:
  - **Success State:** The target cube turns green.
  - **Failure State:** The cube turns red.

---

## Key Highlights
- Implementation of PPO with **continuous action spaces** for smooth navigation.
- Dynamic pathfinding in a constantly changing environment.
- Demonstrates how reinforcement learning algorithms solve real-world dynamic problems.

---

## Project Structure
```
Pathfinding-Ball-PPO/
├── Assets/                # Unity project files (3D environment, materials, scripts)
├── configs/               # YAML configuration files
├── logs/                  # Training logs (used for TensorBoard)
├── models/                # Saved RL models
├── scripts/               # Python scripts for PPO algorithm
├── README.md              # Project documentation
└── requirements.txt       # Dependencies
```

---

## Getting Started

### Prerequisites
- Python 3.8+
- Unity 2021.3+
- Required Python libraries (install via `requirements.txt`):
  ```
  pip install -r requirements.txt
  ```

### Running the Training
1. Set up the Unity environment using the provided `Assets/` folder.
2. Configure training parameters in the `configs/ppo_config.yaml` file.
3. Start training:
   ```bash
   python train.py --config configs/ppo_config.yaml
   ```

### Monitoring
- Launch TensorBoard to visualize training metrics:
  ```bash
  tensorboard --logdir=logs/
  ```

---

## Demo Video
For a visual overview of the project, watch the screen recording:  
**[MY_Project_video](https://unidebhu-my.sharepoint.com/personal/sadman_mailbox_unideb_hu/_layouts/15/stream.aspx?id=%2Fpersonal%2Fsadman%5Fmailbox%5Funideb%5Fhu%2FDocuments%2FMell%C3%A9kletek%2FScreen%20Recording%202024%2D11%2D23%20080824%2Emp4&ct=1733649003075&or=OWA%2DNT%2DMail&cid=7ce70e3d%2De5ec%2D1008%2Dc080%2D2d306e48b005&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E1db602aa%2D6805%2D4daf%2Dbc91%2D17cfcc792704)**

---

## Future Work
- Incorporating additional environmental complexities (e.g., moving obstacles, varying terrain).
- Exploring alternative RL algorithms (e.g., SAC, DDPG).
- Enhancing the dynamic feedback system with auditory cues.

---

## License
This project is licensed under the MIT License.  

Feel free to contribute or reach out for collaboration opportunities! 🚀
