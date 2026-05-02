<div align="center">

# 🎯 CLI - VIDPILOT

**A CLI-based automation agent that searches, navigates, and plays YouTube content — no manual input required.**

[![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![Selenium](https://img.shields.io/badge/Selenium-WebAutomation-green?style=for-the-badge&logo=selenium)](https://www.selenium.dev/)
[![CLI](https://img.shields.io/badge/CLI-InquirerPy-orange?style=for-the-badge)](https://inquirerpy.readthedocs.io/)
[![Agent](https://img.shields.io/badge/Type-Autonomous_Agent-red?style=for-the-badge)](https://github.com/loisekk)
[![License](https://img.shields.io/badge/License-MIT-lightgrey?style=for-the-badge)](LICENSE)
[![Author](https://img.shields.io/badge/Author-Yash%20Brahmankar-success?style=for-the-badge)](https://github.com/loisekk)

> *"An autonomous agent that finds and plays YouTube content — so you don't have to."* 🤖▶️

</div>

---

## 📌 Overview

**VidPilot** is a Python automation agent that removes the friction from YouTube search.

Instead of typing queries manually, the user selects a category and context via an interactive CLI — VidPilot constructs an optimized search query, launches the browser, and plays the most relevant result automatically.

This project demonstrates real-world agentic behavior: decision making, context-aware query generation, and browser automation — packaged in a clean, modular Python architecture.

---

## ✨ Features

| Feature | Details |
|---|---|
| 🎯 Category-Based Search | Structured input replaces raw search typing |
| 🧠 Autonomous Query Building | Context questions → cleaned, optimized query |
| 🤖 Browser Automation | Selenium navigates and plays without user input |
| ⌨️ Interactive CLI | InquirerPy menus for smooth terminal UX |
| 🔍 Query Optimization | Regex-based cleaner removes noise before search |
| 🧩 Modular Architecture | Each category has its own flow module |

---

## 🧠 Supported Categories

| Category | Context Inputs |
|---|---|
| 🏎 F1 Racing | Year, Grand Prix, Stage |
| 🍥 Anime | Title, Type (Intro / Trailer / Clip) |
| 🎬 Movies | Title, Genre |
| 📺 Web Series | Title, Episode |
| 🎮 Gaming | Game name, Content type |
| 🎨 Animations | Style, Topic |
| 🐭 Cartoons | Show name |
| 📘 Study & Tech | Subject, Topic, Level |

---

## ⚙️ How It Works

```
User picks category (CLI)
        ↓
VidPilot asks contextual questions
        ↓
Answers → Query Cleaner (Regex)
        ↓
Selenium opens YouTube → searches → selects top result → plays
        ↓
Agent continues navigation autonomously
```

**Architecture:**

```
┌──────────────┐
│  User CLI    │   ← InquirerPy menus
└──────┬───────┘
       ↓
┌──────────────────┐
│ Category Router  │   ← Picks flow module
└──────┬───────────┘
       ↓
┌──────────────────┐
│ Contextual Flow  │   ← Asks relevant questions per category
└──────┬───────────┘
       ↓
┌──────────────────┐
│ Query Cleaner    │   ← Regex optimization
└──────┬───────────┘
       ↓
┌──────────────────┐
│ Selenium Agent   │   ← Open → Search → Click → Play
└──────────────────┘
```

---

## 🛠 Tech Stack

| Layer | Tool | Purpose |
|---|---|---|
| Language | Python 3.x | Core agent logic |
| Browser Automation | Selenium + ChromeDriver | YouTube navigation & playback |
| CLI UX | InquirerPy | Interactive terminal menus |
| Query Cleaning | `re` (Regex) | Normalize and optimize search strings |
| Config | `python-dotenv` | Environment variable management |

---

## 📂 Project Structure

```
VidPilot/
├── agent.py                  # Entry point — boots CLI and routes to flows
├── flows/
│   ├── anime_flow.py         # Anime category questions + query builder
│   ├── f1_flow.py            # F1 category questions + query builder
│   ├── gaming_flow.py        # Gaming category questions + query builder
│   └── study_flow.py         # Study/Tech category questions + query builder
├── utils/
│   └── query_cleaner.py      # Regex-based query normalization
├── .env                      # Environment config (browser path, etc.)
└── README.md
```

---

## 🚀 Getting Started

**Clone the repo:**

```bash
git clone https://github.com/loisekk/VidPilot.git
cd VidPilot
```

**Install dependencies:**

```bash
pip install selenium inquirerpy python-dotenv
```

**Set up ChromeDriver:**

> Download [ChromeDriver](https://chromedriver.chromium.org/downloads) matching your Chrome version and add it to PATH.

**Run the agent:**

```bash
python agent.py
```

---

## 🎯 Use Cases

- Autonomous agent demos for portfolios
- Selenium + CLI UX practice
- AI/Agentic systems learning
- YouTube research automation
- Template for category-driven CLI tools

---



## 👨‍💻 Author

**Yash Brahmankar**
B.Tech AI & ML | OIST, 2024–2028

[![GitHub](https://img.shields.io/badge/GitHub-loisekk-181717?style=flat-square&logo=github)](https://github.com/loisekk)
[![Email](https://img.shields.io/badge/Email-yashbrahmankar95@gmail.com-D14836?style=flat-square&logo=gmail)](mailto:yashbrahmankar95@gmail.com)

---

## 📄 License

Licensed under the [MIT License](LICENSE) — free to use, modify, and distribute.

---

<div align="center">
  <sub>Built with Python · Powered by Selenium · Driven by InquirerPy</sub>
</div>
