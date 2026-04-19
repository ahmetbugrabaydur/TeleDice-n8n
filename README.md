<p align="center">
  <img src="https://github.com/user-attachments/assets/79e3e4ac-c892-4608-898e-664d8838d029" width="600">
</p>

<h1 align="center">🎲 TeleDice-n8n</h1>

A professional, automated dice-rolling bot for **Dungeons & Dragons** (and other TTRPGs) built entirely with **n8n**. This bot allows players to roll any combination of dice directly within a Telegram chat, making your remote gaming sessions smoother and more interactive.

---

## ✨ Features

* **Multi-Dice Support:** Roll standard D&D dice: `d4`, `d6`, `d8`, `d10`, `d12`, `d20`, and `d100`.
* **Advantage & Disadvantage:** Fully supports D&D 5e mechanics—automatically handles rolling two d20s and selecting the highest or lowest result.
* **Custom Modifiers:** Support for math modifiers like `/roll 1d20 + 5` or `/roll 2d6 - 2`.
* **Instant Response:** Fast processing thanks to n8n's efficient workflow engine.
* **Visual Workflow:** Easy to customize and extend without writing complex backend code.
* **Group Friendly:** Works perfectly in both private messages and Telegram group chats.

## 🛠️ Built With

* **[n8n](https://n8n.io/):** The low-code workflow automation tool used to handle the logic.
* **Telegram Bot API:** For receiving messages and sending roll results.
* **JavaScript (Code Node):** For calculating random dice results, parsing commands, and handling advantage logic.

---

## 🚀 How It Works

1.  **Command Sent:** The user sends a command like `/roll 2d20 + 5` or `/roll d20 adv`.
2.  **Telegram Trigger:** n8n receives the message via a Webhook.
3.  **Regex Parser:** A JavaScript node extracts the number of dice, the type of dice, modifiers, and special tags (adv/dis).
4.  **Dice Logic:** The bot "rolls" the dice, applies math, and calculates the final total.
5.  **Telegram Response:** The final result is sent back to the chat with a clearly formatted message.

---

## 📥 Installation & Setup

1.  **Clone the Repo:** Download the `.json` workflow file from this repository.
2.  **Import to n8n:**
    * Open your n8n instance.
    * Create a new workflow.
    * Click **Import from File** and select the JSON file.
3.  **Telegram Bot Setup:**
    * Create a bot via [@BotFather](https://t.me/botfather) on Telegram to get your **API Token**.
    * In n8n, create a new **Telegram Credential** and paste your token.
4.  **Activate:** Save the workflow and click the **Execute Workflow** or set it to **Active**.

---

## 📝 Usage Examples

<p align="center">
  <img src="https://github.com/user-attachments/assets/88dbf6cb-365b-44bf-b109-198e656a2e1c" width="600" alt="TeleDice Usage Examples">
</p>

* `/roll d20` — Rolls a single 20-sided die.
* `/roll d20 adv` — Rolls with **Advantage** (takes the higher of two rolls).
* `/roll d20 dis` — Rolls with **Disadvantage** (takes the lower of two rolls).
* `/roll 2d6 + 4` — Rolls two 6-sided dice and adds a +4 modifier.
* `/roll 1d100` — For those critical percentile checks!
---

## 🤝 Contributing

Feel free to fork this project, report issues, or submit pull requests to add new features like character sheet integration or expanded combat rules!

**Happy Rolling! 🐉⚔️**
