# python-mooc-journey
My Python learning journey via the University of Helsinki MOOC - one project per part, built on both laptop and my phone, synced through Git.

# 🐍 My Python Learning Journey — University of Helsinki MOOC

> Following the [Python Programming MOOC](https://programming.mooc.fi/) by the University of Helsinki, building a project for every part to practice what I learn — then finishing with four capstone projects that put it all together.

![Progress](https://img.shields.io/badge/Progress-0%2F14%20Parts-red)
![Language](https://img.shields.io/badge/Language-Python-blue)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)

---

## 👋 Why This Exists

I've tried learning Python a few times. This time I'm doing it differently — building real projects as I go, committing everything publicly, and documenting my progress. This repo is the home base that links to every project I build along the way.

The goal isn't just to finish a course. It's to get genuinely comfortable with Python and prove it by shipping things.

---

## 🗺️ Journey Map — MOOC Projects

| Part | Concepts Covered | Project | Status |
|------|-----------------|---------|--------|
| Part 1 | Variables, printing, basic input | [CLI Personal Card](https://github.com/yourusername/cli-personal-card) | 📅 Upcoming |
| Part 2 | Conditionals, loops | [Number Guessing Game](https://github.com/yourusername/number-guessing-game) | 📅 Upcoming |
| Part 3 | Functions | [Unit Converter Tool](https://github.com/yourusername/unit-converter) | 📅 Upcoming |
| Part 4 | Lists, strings | [Expense Tracker](https://github.com/yourusername/expense-tracker) | 📅 Upcoming |
| Part 5 | Dictionaries, tuples | [Contact Book CLI](https://github.com/yourusername/contact-book-cli) | 📅 Upcoming |
| Part 6 | Files, error handling | [Habit Tracker](https://github.com/yourusername/habit-tracker) | 📅 Upcoming |
| Part 7 | Modules, larger programs | [Weather CLI App](https://github.com/yourusername/weather-cli) + [Web Scraper](https://github.com/yourusername/web-scraper) | 📅 Upcoming |
| Part 8 | Classes, OOP basics | [Library Book Manager](https://github.com/yourusername/library-book-manager) | 📅 Upcoming |
| Part 9 | Objects, more OOP | [RPG Character System](https://github.com/yourusername/rpg-character-system) | 📅 Upcoming |
| Part 10 | Class hierarchies, advanced OOP | [Task Manager App](https://github.com/yourusername/task-manager) | 📅 Upcoming |
| Part 11 | List comprehensions, functional tools | [Data Analyzer](https://github.com/yourusername/data-analyzer) | 📅 Upcoming |
| Part 12 | Generators, advanced data structures | [News Headline Fetcher](https://github.com/yourusername/news-fetcher) + [Simple Web Service & API](https://github.com/yourusername/simple-web-api) | 📅 Upcoming |
| Part 12+ | Automation & downloading | [Bulk Downloader](https://github.com/yourusername/bulk-downloader) | 📅 Upcoming |
| Part 13 | pygame basics | [Snake Game](https://github.com/yourusername/snake-game) | 📅 Upcoming |
| Part 14 | Larger pygame project | [Breakout Game](https://github.com/yourusername/breakout-game) | 📅 Upcoming |
| Part 7+ | External libraries, HTTP, networking | [Prank Toolkit 🎭](https://github.com/yourusername/prank-toolkit) | 📅 Upcoming |

**Status legend:** ✅ Done &nbsp;|&nbsp; 🔄 In Progress &nbsp;|&nbsp; 📅 Upcoming

---

## 🏆 Capstone Projects — After the MOOC

These are the four larger projects I'll build once I'm comfortable with Python. Each one pulls together multiple concepts and is scoped like a real-world tool.

| Project | What It Is | Status |
|---------|-----------|--------|
| [Personal Automation Suite](https://github.com/yourusername/personal-automation-suite) | A collection of scripts that automate repetitive tasks — file organization, scheduled reminders, batch renaming, email summaries, etc. | 📅 Upcoming |
| [Network Discovery Tool](https://github.com/yourusername/network-discovery-tool) | Scans a local network to discover connected devices, open ports, and basic info. Uses `socket` and `scapy`. | 📅 Upcoming |
| [System Configuration Manager](https://github.com/yourusername/system-config-manager) | A CLI tool to manage, backup, and restore system/app config files (`.json`, `.ini`, `.toml`). Supports profiles and diffing. | 📅 Upcoming |
| [Simple Web Service + Web API](https://github.com/yourusername/simple-web-api) | A lightweight REST API built with Flask or FastAPI. Serves real data, handles routes, and can be consumed by other tools. | 📅 Upcoming |

---

### 📌 Capstone Project Roadmaps

<details>
<summary><strong>🤖 Personal Automation Suite</strong></summary>

**Core idea:** One repo, multiple automation scripts you actually use day-to-day.

**What it'll include:**
- File organizer — automatically sorts downloads folder by file type
- Bulk file renamer — rename files by pattern, date, or sequence
- Scheduled reminder system — reads a task list and sends desktop notifications
- Email digest — scrapes or fetches content and sends a daily summary email
- Clipboard manager — tracks clipboard history to a log file

**Key libraries:** `os`, `shutil`, `schedule`, `smtplib`, `plyer`, `pathlib`

**Why it stands out:** It's not one project — it's a *suite*. Shows sustained effort and that you build things you actually use.
</details>

<details>
<summary><strong>🌐 Network Discovery Tool</strong></summary>

**Core idea:** Run it on your local network and get a map of everything connected — IPs, hostnames, open ports, device types.

**What it'll include:**
- Ping sweep to find live hosts on a subnet
- Port scanner for common ports (22, 80, 443, 8080, etc.)
- Hostname and MAC address resolution
- Output as a clean table in the terminal or exported to CSV
- Optional: simple Flask UI to view results in a browser

**Key libraries:** `socket`, `scapy`, `ipaddress`, `concurrent.futures` (for speed), `rich` (for pretty terminal output)

**Why it stands out:** Network tools show you understand how computers actually talk to each other. Immediately interesting to anyone in tech or security.
</details>

<details>
<summary><strong>⚙️ System Configuration Manager</strong></summary>

**Core idea:** A CLI tool that manages config files for your apps and system — like a personal dotfiles manager with superpowers.

**What it'll include:**
- Load, read, and edit `.json`, `.ini`, and `.toml` config files
- Save named profiles (e.g. "work", "home", "dev")
- Switch between profiles instantly
- Backup configs before changes and restore from backup
- Diff two configs to see what changed

**Key libraries:** `configparser`, `tomllib`/`tomli`, `json`, `argparse`, `difflib`, `shutil`

**Why it stands out:** Every developer deals with config files. Building a tool to manage them shows you understand real developer pain points.
</details>

<details>
<summary><strong>🔌 Simple Web Service + Web API</strong></summary>

**Core idea:** Build an API that actually *serves* data — the flip side of consuming APIs, which you'll have done throughout the MOOC.

**What it'll include:**
- REST API with GET, POST, PUT, DELETE routes
- A real dataset behind it (could be your expense data, a book list, anything)
- Basic authentication with API keys
- JSON responses with proper status codes
- Simple documentation page (auto-generated with FastAPI)
- Optional: connect it to your News Fetcher or Data Analyzer as the data source

**Key libraries:** `FastAPI` or `Flask`, `uvicorn`, `pydantic`, `sqlite3` or `json` for storage

**Why it stands out:** Most beginners only ever *consume* APIs. Building one shows a completely different level of understanding and opens the door to backend development.
</details>

---

## 🎭 Just For Fun — Prank Toolkit

Not everything has to be serious. This repo is a collection of Python-powered pranks built with real libraries and real networking concepts — just aimed at chaos.

| Tool | What It Does |
|------|--------------|
| `rickroll_qr.py` | Generates a QR code that rickrolls whoever scans it |
| `audio_qr.py` | QR code that plays a custom sound in the browser when scanned |
| `jumpscare_qr.py` | QR code that opens a jumpscare or funny page |
| `network_trigger.py` | Connects to VirtualDJ's HTTP API over WiFi and fires play commands |
| `remote_control.py` | A secret Flask page with a big red button that drops a prank song into a live DJ set |
| `crowd_qr.py` | QR code that blasts audio through everyone's phones simultaneously |

> ⚠️ All pranks performed with full permission. Probably.

🔗 **[prank-toolkit repo →](https://github.com/yourusername/prank-toolkit)**

---

## 🧠 What I'm Learning Along the Way

<!-- Update this section as you go -->

- **Part 1:** _(e.g. "Learned how Python handles types differently from what I expected")_
- **Part 2:** _(your reflection here)_

---

## 🛠️ Tools & Libraries Used

<!-- Fill this in as you use them -->

- `requests` — API calls & web scraping
- `yt-dlp` — video/bulk downloading
- `pygame` — game development
- `flask` / `fastapi` — web services
- `scapy` — network tools
- `qrcode` — QR code generation
- `flask` — prank remote control web page
- `csv` / `json` — file handling
- _(more to come...)_

---

## 📁 How Each Project Repo Is Structured

Every project repo follows this structure:
```
project-name/
├── main.py
├── README.md        ← what it does, how to run it, what I learned
├── requirements.txt ← if any external libraries are needed
└── screenshots/     ← for visual projects
```

---

## 🔗 Connect

- GitHub: [@yourusername](https://github.com/yourusername)
- _(add Twitter/LinkedIn/etc if you want)_

---

> "The best time to start was years ago. The second best time is now." 🚀
