# ♟️ Conversational Chess using Nested Chat Agents

An innovative AI-based chess interface where you play or discuss chess through **natural conversation**. Powered by **nested chat agents**, this project aims to make learning, analyzing, and playing chess more interactive and intelligent.

## 🔍 Project Description

This project demonstrates how nested conversational agents can simulate chess gameplay, guide users through moves, explain strategies, and even correct mistakes—all in a natural language format.

### ✨ Features

- Play chess via chat commands (e.g., "Move my knight to f3")
- Receive hints, rules, and move suggestions
- Nested agents for handling:
  - Game rules
  - Move validation
  - Strategy advice
  - Contextual memory and planning
- Interactive, text-based interface

## 🧠 Tech Stack

- **Language**: Python
- **Framework**: [AutoGen](https://github.com/microsoft/autogen)
- **Memory Integration**: Zep long-term memory (optional)
- **Chess Logic**: `python-chess` or custom implementation
- **LLM Integration**: OpenAI GPT agents
- **Nested Agents**: AutoGen `ConversableAgent`, `GroupChat`, `GroupChatManager`

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/jeevangowda1718/Coversational-Chess-using-Nested-Chat.git
   cd Coversational-Chess-using-Nested-Chat

    Install dependencies:

pip install -r requirements.txt

Add your OpenAI API key in the config:

# llm_config = {
#     "config_list": [{"model": "gpt-4", "api_key": "your-openai-api-key"}]
# }

Run the agent:

    python main.py

🧩 Example Interactions

User: What's the best move in this position?
Agent: Considering your bishop and queen alignment, moving your bishop to g5 could pressure the king's defense.

User: Move my pawn to e4
Agent: Move accepted. It's your opponent's turn.

📁 Project Structure

├── main.py                     # Main entry point
├── chess_agent.py              # Chess move logic and validation
├── strategy_agent.py           # Strategy explanation module
├── zep_conversable_agent.py    # Memory-integrated agents
├── llm_config.py               # LLM setup
└── README.md                   # Project overview
