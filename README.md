# My Python Learning Journey — University of Helsinki MOOC

> Following the [Python Programming MOOC](https://programming.mooc.fi/) by the University of Helsinki, building a project for every part to practice what I learn — then finishing with four capstone projects that put it all together.

![Progress](https://img.shields.io/badge/Progress-0%2F14%20Parts-red)
![Language](https://img.shields.io/badge/Language-Python-blue)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
![Laptop](https://img.shields.io/badge/Laptop-Linux-orange)
![Phone](https://img.shields.io/badge/Phone-Android%20%2B%20Termux-green)

---

## Why This Exists

I've tried learning Python a few times. This time I'm doing it differently — building real projects as I go, committing everything publicly, and documenting my progress. This repo is the home base that links to every project I build along the way.

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

## Journey Map — MOOC Projects

All MOOC projects live inside this repo under the mooc/ folder.

| Part | Concepts Covered | Project | Status |
|------|-----------------|---------|--------|
| Part 1 | Variables, printing, basic input | [CLI Personal Card](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-01-cli-personal-card) | Upcoming |
| Part 2 | Conditionals, loops | [Number Guessing Game](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-02-number-guessing-game) | Upcoming |
| Part 3 | Functions | [Unit Converter Tool](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-03-unit-converter) | Upcoming |
| Part 4 | Lists, strings | [Expense Tracker](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-04-expense-tracker) | Upcoming |
| Part 5 | Dictionaries, tuples | [Contact Book CLI](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-05-contact-book-cli) | Upcoming |
| Part 6 | Files, error handling | [Habit Tracker](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-06-habit-tracker) | Upcoming |
| Part 7 | Modules, larger programs | [Weather CLI App](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-07-weather-cli) + [Web Scraper](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-07-web-scraper) | Upcoming |
| Part 8 | Classes, OOP basics | [Library Book Manager](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-08-library-book-manager) | Upcoming |
| Part 9 | Objects, more OOP | [RPG Character System](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-09-rpg-character-system) | Upcoming |
| Part 10 | Class hierarchies, advanced OOP | [Task Manager App](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-10-task-manager) | Upcoming |
| Part 11 | List comprehensions, functional tools | [Data Analyzer](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-11-data-analyzer) | Upcoming |
| Part 12 | Generators, advanced data structures | [News Headline Fetcher](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-12-news-fetcher) + [Simple Web Service & API](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-12-simple-web-api) | Upcoming |
| Part 12+ | Automation & downloading | [Bulk Downloader](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-12-bulk-downloader) | Upcoming |
| Part 13 | pygame basics | [Snake Game](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-13-snake-game) | Upcoming |
| Part 14 | Larger pygame project | [Breakout Game](https://github.com/damechi-dot/python-mooc-journey/tree/main/mooc/part-14-breakout-game) | Upcoming |
| Part 7+ | External libraries, HTTP, networking | [Prank Toolkit 🎭](https://github.com/damechi-dot/python-mooc-journey/tree/main/fun/prank-toolkit) | Upcoming |

---