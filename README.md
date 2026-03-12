# My Python Learning Journey — University of Helsinki MOOC

> Following the [Python Programming MOOC](https://programming-26.mooc.fi/) by the University of Helsinki, building a project for every part to practice what I learn — then finishing with four capstone projects that put it all together.

![Progress](https://img.shields.io/badge/Progress-0%2F14%20Parts-red)
![Language](https://img.shields.io/badge/Language-Python-blue)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
![Laptop](https://img.shields.io/badge/Laptop-Linux-orange)
![Phone](https://img.shields.io/badge/Phone-Android%20%2B%20Termux-green)

---

## Why This Exists

I've tried learning Python a few times. This time I'm doing it differently by building real projects as I go, saving my own solutions to every exercise, committing everything publicly, and documenting my progress. This repo is the home base that links to everything I build along the way.

The goal isn't just to finish a course. It's to get genuinely comfortable with Python and prove it by shipping things.

---

## 💻📱 How I Code — Dual Device Setup

One of the real challenges in my learning journey is inconsistent access to electricity. So I built a setup that lets me code from anywhere — on my laptop when power is available, and on my Android phone when it's not. Everything stays in sync through Git and GitHub.

| | Laptop | Phone |
|--|--------|-------|
| **OS** | Linux (Ubuntu 24.04 LTS) | Android (XOS) |
| **Editor** | VS Code | Pydroid 3 |
| **Terminal** | Bash | Termux |
| **Git** | Git CLI | Git CLI (Termux) |
| **Use case** | Full scale building, complex projects, games | Quick edits, continuing work, small scripts, Git sync |

### 📱 Phone Stack
- **Pydroid 3** — write and run Python with one tap, works fully offline
- **Termux** — Git operations (`pull`, `push`, `commit`) and quick terminal access
- **Acode** — file browsing and navigation across the project folder
- **GitHub Mobile** — monitor repos and commits on the go

### 🔄 Sync Workflow
Both devices share the exact same repo cloned from GitHub. The golden rule:

> **Pull before you start. Push before you stop. Every single time.**

```
Phone ──push──► GitHub ◄──push── Laptop
      ◄──pull──         ──pull──►
```

For the full device setup guide including installation steps, SSH key configuration, and folder structure — see [SETUP.md](./SETUP.md).

---

## Journey Map. Folder Structure + MOOC Projects

Everything lives inside this one repo (exercises and projects), organized by category, one folder per part. Everything is identical on both my laptop and phone, synced through Git.

```
python-mooc-journey/           ← main GitHub repo
│
├── README.md                  ← you are here (the main repo readme file)
├── SETUP.md                   ← full guide to my dual device setup
│
└── mooc/
    ├── part-01/
    │   ├── exercises/         ← my solutions to part 1 MOOC exercises
    │   ├── project/           ← CLI Personal Card
    │   └── README.md          ← what I built, what I learned
    ├── part-02/
    │   ├── exercises/         ← my solutions to part 2 MOOC exercises
    │   ├── project/           ← Number Guessing Game
    │   └── README.md
    ├── part-03/
    │   ├── exercises/         ← my solutions to part 3 MOOC exercises
    │   ├── project/           ← Unit Converter Tool
    │   └── README.md
    ├── part-04/
    │   ├── exercises/         ← my solutions to part 4 MOOC exercises
    │   ├── project/           ← Expense Tracker
    │   └── README.md
    ├── part-05/
    │   ├── exercises/         ← my solutions to part 5 MOOC exercises
    │   ├── project/           ← Contact Book CLI
    │   └── README.md
    ├── part-06/c
    │   ├── exercises/         ← my solutions to part 6 MOOC exercises
    │   ├── project/           ← Habit Tracker
    │   └── README.md
    ├── part-07/
    │   ├── exercises/         ← my solutions to part 7 MOOC exercises
    │   ├── project/           ← Weather CLI + Web Scraper
    │   └── README.md
    ├── part-08/
    │   ├── exercises/         ← my solutions to part 8 MOOC exercises
    │   ├── project/           ← Library Book Manager
    │   └── README.md
    ├── part-09/
    │   ├── exercises/         ← my solutions to part 9 MOOC exercises
    │   ├── project/           ← RPG Character System
    │   └── README.md
    ├── part-10/
    │   ├── exercises/         ← my solutions to part 10 MOOC exercises
    │   ├── project/           ← Task Manager App
    │   └── README.md
    ├── part-11/
    │   ├── exercises/         ← my solutions to part 11 MOOC exercises
    │   ├── project/           ← Data Analyzer
    │   └── README.md
    ├── part-12/
    │   ├── exercises/         ← my solutions to part 12 MOOC exercises
    │   ├── project/           ← News Fetcher + Web API + Bulk Downloader
    │   └── README.md
    ├── part-13/
    │   ├── exercises/         ← my solutions to part 13 MOOC exercises
    │   ├── project/           ← Snake Game
    │   └── README.md
    └── part-14/
        ├── exercises/         ← my solutions to part 14 MOOC exercises
        ├── project/           ← Breakout Game
        └── README.md
```

🔗 Capstone projects live in a separate repo — capstone-projects →
🔗 Fun projects live in a separate repo — prank-toolkit →

---

## 🗺️ Course 1 — Introduction to Programming (Parts 1–7)

> 📖 [Course link](https://programming-26.mooc.fi/) &nbsp;|&nbsp; Parts 1 through 7

| Part | Topics | Exercises | Project | Status |
|------|--------|-----------|---------|--------|
| [Part 1](https://programming-26.mooc.fi/part-1) | Variables, printing, input, arithmetic | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-01/exercises) | [CLI Personal Card](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-01/project) | In Progress |
| [Part 2](https://programming-26.mooc.fi/part-2) | Conditionals, loops, basic logic | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-02/exercises) | [Number Guessing Game](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-02/project) | Upcoming |
| [Part 3](https://programming-26.mooc.fi/part-3) | Functions, loops revisited | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-03/exercises) | [Unit Converter Tool](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-03/project) | Upcoming |
| [Part 4](https://programming-26.mooc.fi/part-4) | Lists, strings | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-04/exercises) | [Expense Tracker](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-04/project) | Upcoming |
| [Part 5](https://programming-26.mooc.fi/part-5) | Dictionaries, tuples | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-05/exercises) | [Contact Book CLI](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-05/project) | Upcoming |
| [Part 6](https://programming-26.mooc.fi/part-6) | Files, error handling | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-06/exercises) | [Habit Tracker](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-06/project) | Upcoming |
| [Part 7](https://programming-26.mooc.fi/part-7) | Modules, larger programs | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-07/exercises) | [Weather CLI](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-07/project) + [Web Scraper](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-07/project) | Upcoming |

---

## 🗺️ Course 2 — Advanced Course in Programming (Parts 8–14)

> 📖 [Course link](https://programming-26.mooc.fi/) &nbsp;|&nbsp; Parts 8 through 14

| Part | Topics | Exercises | Project | Status |
|------|--------|-----------|---------|--------|
| [Part 8](https://programming-26.mooc.fi/part-8) | Classes, OOP basics | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-08/exercises) | [Library Book Manager](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-08/project) | Upcoming |
| [Part 9](https://programming-26.mooc.fi/part-9) | Objects, more OOP | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-09/exercises) | [RPG Character System](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-09/project) | Upcoming |
| [Part 10](https://programming-26.mooc.fi/part-10) | Class hierarchies, advanced OOP | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-10/exercises) | [Task Manager App](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-10/project) | Upcoming |
| [Part 11](https://programming-26.mooc.fi/part-11) | List comprehensions, functional tools | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-11/exercises) | [Data Analyzer](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-11/project) | Upcoming |
| [Part 12](https://programming-26.mooc.fi/part-12) | Generators, advanced data structures | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-12/exercises) | [News Fetcher](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-12/project) + [Web API](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-12/project) + [Bulk Downloader](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-12/project) | Upcoming |
| [Part 13](https://programming-26.mooc.fi/part-13) | pygame basics | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-13/exercises) | [Snake Game](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-13/project) | Upcoming |
| [Part 14](https://programming-26.mooc.fi/part-14) | Larger pygame project | [exercises](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-14/exercises) | [Breakout Game](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-14/project) | Upcoming |

---


## Capstone Projects — After the MOOC

These are the four larger projects I'll build once I'm comfortable with Python. They all live inside one dedicated `capstone-projects` repo and each pulls together multiple concepts and is scoped like a real-world tool.

🔗 **[capstone-projects repo →](https://github.com/damechi-dot/capstone-projects)**

| Project | What It Is |
|---------|-----------|
| [Personal Automation Suite](https://github.com/damechi-dot/capstone-projects/tree/main/personal-automation-suite) | A collection of scripts that automate repetitive tasks — file organization, scheduled reminders, batch renaming, email summaries, etc. |
| [Network Discovery Tool](https://github.com/damechi-dot/capstone-projects/tree/main/network-discovery-tool) | Scans a local network to discover connected devices, open ports, and basic info. Uses `socket` and `scapy`. |
| [System Configuration Manager](https://github.com/damechi-dot/capstone-projects/tree/main/system-config-manager) | A CLI tool to manage, backup, and restore system/app config files (`.json`, `.ini`, `.toml`). Supports profiles and diffing. |
| [Simple Web Service + Web API](https://github.com/damechi-dot/capstone-projects/tree/main/simple-web-api) | A lightweight REST API built with Flask or FastAPI. Serves real data, handles routes, and can be consumed by other tools. |

---

## Just For Fun — Prank Toolkit

Not everything has to be serious. This repo is a collection of Python-powered pranks built with real libraries and real networking concepts — just aimed at chaos.

🔗 **[prank-toolkit repo →](https://github.com/damechi-dot/prank-toolkit)**

| Tool | What It Does |
|------|--------------|
| `rickroll_qr.py` | Generates a QR code that rickrolls whoever scans it |
| `audio_qr.py` | QR code that plays a custom sound in the browser when scanned |
| `jumpscare_qr.py` | QR code that opens a jumpscare or funny page |
| `network_trigger.py` | Connects to VirtualDJ's HTTP API over WiFi and fires play commands |
| `remote_control.py` | A secret Flask page with a big red button that drops a prank song into a live DJ set |
| `crowd_qr.py` | QR code that blasts audio through everyone's phones simultaneously |

> ⚠️ All pranks performed with full permission. Probably.

---

## 🧠 What I'm Learning Along the Way

`UPDATING...`

<!-- Update this section as you go -->
<!--
- **Part 1:** _(e.g. "Learned how Python handles types differently from what I expected")_
- **Part 2:** _(your reflection here)_ -->

---

## 🛠️ Tools & Libraries Used

`UPCOMING...`

<!-- Fill this in as you use them -->
<!--
- `requests` — API calls & web scraping
- `yt-dlp` — video/bulk downloading
- `pygame` — game development
- `flask` / `fastapi` — web services
- `scapy` — network tools
- `qrcode` — QR code generation
- `csv` / `json` — file handling
- _(more to come...)_ -->

---

## 🔗 Connect

- GitHub: [@damechi-dot](https://github.com/damechi-dot)
- X/Twitter: [@heydamechi](https://x.com/heydamechi)
<!-- _(add Twitter/LinkedIn/etc if you want)_ -->

---

> "The best time to start was years ago. The second best time is now." 🚀