# 📱💻 My Dev Environment Setup Guide
### Python MOOC — Linux Laptop + Android Phone (Termux)

> This guide sets up a coding environment on both devices and keeps everything in sync through GitHub. Written for beginners — every command is explained.

---

## 📁 Folder Structure

This is how my folder structure looks, yours could be different but you get the hint. It's identical on both laptop and phone.

```
python-mooc-journey/              ← main GitHub repo
│
├── README.md                     ← the main repo readme file
├── SETUP.md                      ← this file
│
├── mooc/                         ← all MOOC part projects live here
│   ├── part-01-cli-personal-card/
│   │   ├── main.py
│   │   ├── README.md
│   │   └── screenshots/
│   ├── part-02-number-guessing-game/
│   │   ├── main.py
│   │   └── README.md
│   ├── part-03-unit-converter/...
│   ├── part-04-expense-tracker/...
│   ├── part-05-contact-book/...
│   ├── part-06-habit-tracker/...
│   ├── part-07-weather-cli/...
│   ├── part-07-web-scraper/...
│   ├── part-08-library-manager/...
│   ├── part-09-rpg-system/...
│   ├── part-10-task-manager/...
│   ├── part-11-data-analyzer/...
│   ├── part-12-news-fetcher/...
│   ├── part-12-web-api/...
│   ├── part-12-bulk-downloader/...
│   ├── part-13-snake-game/...
│   └── part-14-breakout-game/...
├── 
```

---

## 💻 Laptop Setup (Linux)

### Step 1 — Install Git & Python (if not already)
```bash
sudo apt update
sudo apt install git python3 python3-pip -y
```

Verify they installed:
```bash
python3 --version
git --version
```

### Step 2 — Configure Git
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### Step 3 — Generate SSH Key for GitHub
This means you'll never have to type your GitHub password again:
```bash
ssh-keygen -t ed25519 -C "your@email.com"
# Press Enter for all prompts (use default location, no passphrase is fine)

# Now view your public key and copy it
cat ~/.ssh/id_ed25519.pub
```

Go to **GitHub → Settings → SSH and GPG Keys → New SSH Key** → paste it in → Save.

Test it worked:
```bash
ssh -T git@github.com
# Should say: "Hi yourusername! You've successfully authenticated"
```

### Step 4 — Create the Repo on GitHub
1. Go to github.com → New Repository
2. Name it `python-mooc-journey`
3. Make it Public
4. Check "Add a README file"
5. Click Create

### Step 5 — Clone it to Your Laptop
```bash
cd ~
mkdir projects
cd projects
git clone git@github.com:yourusername/python-mooc-journey.git
cd python-mooc-journey
```

### Step 6 — Create the Folder Structure
Run this once to create all the folders in one go:
```bash
# MOOC folders
mkdir -p mooc/part-01-cli-personal-card/screenshots
mkdir -p mooc/part-02-number-guessing-game
mkdir -p mooc/part-03-unit-converter
mkdir -p mooc/part-04-expense-tracker
mkdir -p mooc/part-05-contact-book
mkdir -p mooc/part-06-habit-tracker
mkdir -p mooc/part-07-weather-cli
mkdir -p mooc/part-07-web-scraper
mkdir -p mooc/part-08-library-manager
mkdir -p mooc/part-09-rpg-system
mkdir -p mooc/part-10-task-manager
mkdir -p mooc/part-11-data-analyzer
mkdir -p mooc/part-12-news-fetcher
mkdir -p mooc/part-12-web-api
mkdir -p mooc/part-12-bulk-downloader
mkdir -p mooc/part-13-snake-game/screenshots
mkdir -p mooc/part-14-breakout-game/screenshots
```

### Step 7 — Push the Structure to GitHub
Git won't track empty folders, so create a placeholder file in each:
```bash
find . -type d -empty -not -path "./.git/*" -exec touch {}/.gitkeep \;

# Now add, commit and push everything
git add .
git commit -m "initial folder structure"
git push
```

Your folder structure is now live on GitHub. ✅

### Step 8 — VS Code Setup
Open the project in VS Code:
```bash
code .
```

---

## 📱 Phone Setup (Android + Termux)

### Step 1 — Install F-Droid
> ⚠️ Do NOT get Termux from the Play Store — it's outdated. Use F-Droid instead.

1. Go to `https://f-droid.org` in your browser
2. Download and install the F-Droid APK
3. You may need to allow "Install from unknown sources" in your Android settings — it's safe

### Step 2 — Install Termux from F-Droid
1. Open F-Droid
2. Search "Termux"
3. Install it

### Step 3 — Install Required Packages in Termux
Open Termux and run these one by one:
```bash
pkg update && pkg upgrade
# Press Enter/Y when prompted

pkg install python
pkg install git
pkg install openssh
```

Verify:
```bash
python --version
git --version
```

### Step 4 — Configure Git on Termux
Same as laptop:
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### Step 5 — Generate SSH Key on Phone
```bash
ssh-keygen -t ed25519 -C "your@email.com"
# Press Enter for all prompts

# View and copy your key
cat ~/.ssh/id_ed25519.pub
```

Go to **GitHub → Settings → SSH Keys → New SSH Key** → paste it → Save.
(You'll now have two SSH keys in GitHub — one for laptop, one for phone.)

Test it:
```bash
ssh -T git@github.com
```

### Step 6 — Clone Your Repo on the Phone
```bash
mkdir -p ~/projects
cd ~/projects
git clone git@github.com:yourusername/python-mooc-journey.git
cd python-mooc-journey
```

Your full folder structure is now on your phone. ✅

### Step 7 — Install Recommended Apps

| App | Where to Get | What It's For |
|-----|-------------|---------------|
| **Pydroid 3** | Play Store | Running Python files with a GUI |
| **Pydroid 3 IDE Plugin** | Play Store | Unlocks pip installs inside Pydroid |
| **Acode** | Play Store | Writing code (better editor than Pydroid) |
| **GitHub Mobile** | Play Store | Browsing repos, reviewing changes |
| **Termux:Widget** | F-Droid | Run scripts from your home screen |
| **Termux:API** | F-Droid | Let Python access your phone hardware |

### Step 8 — Point Pydroid at Your Project Folder
When you open a file in Pydroid, navigate to:
```
/data/data/com.termux/files/home/projects/python-mooc-journey/
```
This is where Termux stores your files. Pydroid can open and run files directly from here.

---

## 🔄 Daily Sync Workflow

This is the routine that keeps everything in sync between devices.

### When you finish a session on your LAPTOP:
```bash
cd ~/projects/python-mooc-journey
git add .
git commit -m "brief description of what you did"
git push
```

### When you start a session on your PHONE:
```bash
cd ~/projects/python-mooc-journey
git pull
```

### When you finish a session on your PHONE:
```bash
cd ~/projects/python-mooc-journey
git add .
git commit -m "continued part X on phone"
git push
```

### When you start a session on your LAPTOP:
```bash
cd ~/projects/python-mooc-journey
git pull
```

> 💡 **Golden rule:** always `git pull` before you start and `git push` before you stop. Do this every single time and you'll never have sync conflicts.

---

## 🆘 Common Problems & Fixes

**"Permission denied (publickey)" when pushing**
→ Your SSH key isn't added to GitHub yet. Redo Step 3 (laptop) or Step 5 (phone).

**"Updates were rejected" when pushing**
→ You forgot to pull before starting. Run `git pull` first, then push again.

**Termux says "command not found" for python**
→ Run `pkg install python` again.

**Pydroid can't find your files**
→ Navigate to `/data/data/com.termux/files/home/projects/` inside Pydroid's file browser.

**pip install fails in Termux**
→ Use `pip install packagename` inside Termux directly, not inside Pydroid, for best results.

---

## 📦 Installing Python Packages

**On Laptop:**
```bash
pip install packagename
# or
pip3 install packagename
```

**On Phone (Termux):**
```bash
pip install packagename
```

**On Phone (Pydroid):**
Open the hamburger menu → Pip → search and install from there.

---

> Built for coding anywhere — with or without electricity. 🔋

<small>Written with * by Damechi x Claude</small>