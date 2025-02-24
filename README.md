# **🐍 Reinforcement Learning-Based Snake Game AI Agent**

## **📌 Introduction**
This project implements an **AI agent** using **Reinforcement Learning (Deep Q-Learning - DQN)** to play the classic **Snake game**. The AI is trained through trial and error, gradually improving its performance.

## **📂 Project Structure**
```
Reinforcement-Learning-Snake-Game/
│── model/               # Contains trained models
│── __pycache__/         # Compiled Python files
│── agent.py             # AI agent implementation
│── helper.py            # Utility functions for training and evaluation
│── model.py             # Neural network model definition
│── snake_human.py       # Human-controlled Snake game converted for the AI to play
│── arial.ttf            # Font file for display
│── requirements.txt     # Dependencies list
│── README.md            # Project documentation
│── .gitignore           # Ignored files in Git repository
```

## **🧠 AI Agent Implementation**
The AI agent is developed using **Deep Q-Learning (DQN)**, where a neural network is trained to approximate Q-values and make optimal moves.

- **State Representation:** The agent observes the game grid, food position, and snake direction.
- **Action Space:** The possible actions include turning left, right, or continuing straight.
- **Reward System:**
  - 🟢 **+10** for eating food.
  - 🔴 **-10** for colliding with walls or itself.
  - ⚪ **0** for moving without any significant event.

## **📊 Training Details**
- **Training Episodes:** **350 games**
- **Highest Score:** **75** (achieved at game 222)
- **Observations:** The AI learned to navigate and survive effectively, but improvements plateaued beyond 222 games.

## **📌 Installation & Usage**
### **🔹 Prerequisites**
Make sure you have **Python** installed. Install dependencies using:
```bash
pip install -r requirements.txt
```

### **🔹 Running the AI Agent**
To run the AI-controlled Snake game:
```bash
python agent.py
```

To play manually:
```bash
python snake_human.py
```

## **📈 Results**
- 🏆 The AI successfully learned to play Snake and achieved a high score of **75**.
- 📉 Performance plateaued after **game 224**.
- 🤖 The AI adapted well to the environment but showed diminishing improvements over time.

## **🔍 Future Improvements**
- 🔧 Fine-tuning **hyperparameters** for better learning efficiency.
- 🚀 Increasing **training duration** to enhance performance.
- 📊 Experimenting with **different RL algorithms** like PPO or A3C.

### **💡 Contributing**
Feel free to **fork** this repository and contribute! 🎯

### **📬 Contact**
For any queries, reach out via **GitHub Issues**.
