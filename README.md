# Reinforcement Learning Assignment 2

Coursework exploring reinforcement learning methods in Gymnasium environments. The repository includes notebook implementations of Deep Q-Network (DQN) and Proximal Policy Optimization (PPO) for CartPole and Atari Breakout, plus tabular Q-learning for the continuous Pendulum task.

## Experiments

| Notebook | Environment | Method |
|---|---|---|
| `CartpoleDQN.ipynb` | CartPole-v1 | DQN |
| `CartpolePPO.ipynb` | CartPole-v1 | PPO |
| `BreakoutDQN.ipynb` | ALE/Breakout-v5 | DQN |
| `BreakoutPPO.ipynb` | ALE/Breakout-v5 | PPO |
| `pendulum.ipynb` | Pendulum-v1 | Tabular Q-learning |

The `pendulumQlearning/` directory contains configuration, Q-table checkpoints, training logs, a learning curve, and recorded episodes. Other experiment directories contain training checkpoints, Gym monitor logs, and sample videos. The root also includes the assignment report, specification, and model diagrams.

## Requirements

Use Python 3.10 or newer with Jupyter Notebook/Lab. The notebooks install or use Gymnasium and Stable-Baselines3; Breakout additionally requires the Atari/ALE and ROM support used in its notebook. Rendering or video recording may require FFmpeg and a compatible display backend. Run each notebook from the repository root so relative output paths resolve as expected.

## Run

```bash
python -m venv .venv
# Windows: .venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install notebook
jupyter notebook
```

Open the desired notebook and run its cells in order. Training can take substantial time and may require a GPU for faster image-based Breakout experiments. Notebook cells may install additional dependencies; review and run those setup cells in the active environment.

## Notes

Model checkpoints and recorded videos are included as experiment artifacts. The largest checkpoints are approximately 28 MB each; none of the inspected individual files exceeds 100 MB. Notebook outputs may include embedded video data and make notebooks larger than their source code. The supplied assignment specification is included for reference; follow its original course and distribution terms.
