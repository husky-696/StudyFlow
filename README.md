<div align="center">

# StudyFlow CLI

### Workflow automation for Canvas LMS

Less time navigating dashboards. More time learning.

[![npm version](https://img.shields.io/npm/v/studyflow-bot.svg?style=flat-square)](https://www.npmjs.com/package/studyflow-bot)
[![npm downloads](https://img.shields.io/npm/dm/studyflow-bot.svg?style=flat-square)](https://www.npmjs.com/package/studyflow-bot)
[![Node.js](https://img.shields.io/badge/node-%3E%3D18-brightgreen.svg?style=flat-square)](https://nodejs.org/)
[![License](https://img.shields.io/badge/license-proprietary-blue.svg?style=flat-square)](LICENSE)

</div>

---

## About

StudyFlow is a productivity assistant that automates lecture management on Canvas LMS. Instead of manually tracking videos across courses, StudyFlow organizes your study workflow—so you spend less time managing dashboards and more time actually learning.

**Perfect for students who:**
- Have multiple Canvas courses with scattered video lectures
- Want to stay on top of lecture completion without constant clicking
- Need a simple, automated way to manage study organization
- Prefer a hands-off approach to routine dashboard tasks

---

## Features

✨ **Smart Lecture Management**  
Discovers and organizes video lectures across all your Canvas courses in one place.

🤖 **Automated Workflow**  
Handles routine lecture playback tasks without manual intervention.

🎯 **Study Organization**  
Keeps track of what you've watched and what's left to do.

🌙 **Headless Mode**  
Run silently in the background while you work or study.

👁️ **Visible Mode**  
Watch the process in real-time if you prefer transparency.

🔒 **Privacy First**  
Credentials stay on your machine. No cloud sync. No tracking.

⚡ **Zero Technical Knowledge Required**  
Simple menu-driven interface. No coding needed.

---

## Installation

Choose your operating system below and follow the steps:

---

### 🪟 Windows

#### Step 1: Install Node.js

**Option A: Using Winget (Recommended)**
```bash
winget install OpenJS.NodeJS.LTS
```

**Option B: Manual Download**
1. Visit [nodejs.org](https://nodejs.org)
2. Click the green **"LTS"** button
3. Double-click the `.msi` file that downloads
4. Click **"Next"** through all prompts (keep defaults)
5. Click **"Install"** and wait for completion

#### Step 2: Open PowerShell

1. Press the **Windows key** on your keyboard
2. Type `PowerShell`
3. Click **"Windows PowerShell"** to open

#### Step 3: Install StudyFlow

```bash
npm install -g studyflow-bot
```

Wait for installation to complete (you'll see progress bars).

#### Step 4: Launch

```bash
studyflow
```

Done! Follow the on-screen setup wizard.

---

### 🍎 macOS (Intel & Apple Silicon)

#### Step 1: Install Node.js

**Option A: Using Homebrew (Recommended)**

If you don't have Homebrew installed, first run:
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Then install Node.js:
```bash
brew install node
```

**Option B: Manual Download**
1. Visit [nodejs.org](https://nodejs.org)
2. Click the green **"LTS"** button
3. Choose the macOS installer for your chip:
   - **Intel Chip:** Download the `.pkg` file labeled "Intel"
   - **Apple Silicon (M1/M2/M3):** Download the `.pkg` file labeled "Apple Silicon"
4. Double-click the downloaded `.pkg` file
5. Click **"Continue"** and follow the prompts
6. Click **"Install"** and enter your Mac password if prompted

#### Step 2: Open Terminal

1. Press `Cmd + Space` on your keyboard
2. Type `Terminal`
3. Press `Enter`

#### Step 3: Install StudyFlow

```bash
npm install -g studyflow-bot
```

Wait for installation to complete.

#### Step 4: Launch

```bash
studyflow
```

Done! Follow the on-screen setup wizard.

---

### 🐧 Linux

#### Step 1: Install Node.js

**Ubuntu / Debian:**
```bash
sudo apt update
sudo apt install -y nodejs npm
```

**Fedora / RHEL / CentOS:**
```bash
sudo dnf install -y nodejs npm
```

**Arch Linux:**
```bash
sudo pacman -S nodejs npm
```

**Other Distributions:**
Visit the [Node.js package manager guide](https://nodejs.org/en/download/package-manager/) for your distro.

#### Step 2: Install StudyFlow

```bash
npm install -g studyflow-bot
```

#### Step 3: Launch

```bash
studyflow
```

Done! Follow the on-screen setup wizard.

---

## Quick Start

```bash
# Launch StudyFlow
studyflow

# Follow the setup wizard:
# 1. Enter your Canvas credentials
# 2. Choose your preferred mode (headless or visible)
# 3. Select lectures to manage

# Stop anytime with:
# Ctrl + C
```

---

## First-Time Setup

### License Activation
Enter your unique license key (provided by your institution).

### Canvas Credentials
- **Username:** Your Canvas student ID
- **Password:** Your Canvas password (stored locally, never shared)

### Browser Setup
StudyFlow automatically downloads a lightweight browser engine on first run (~1-2 minutes). This is a one-time download.

### Mode Selection
Choose between:
- **Headless (default):** Run in the background silently
- **Visible:** See the browser window and watch the process

---

## Using StudyFlow

### Headless vs Visible Mode

**Headless Mode** (Default)
- Runs quietly in the background
- Best for: Working on other tasks
- Switch modes anytime via the menu

**Visible Mode**
- Browser window opens so you can watch
- Best for: Troubleshooting or seeing what's happening
- Toggle in the CLI menu: `👁️ Toggle Headless Mode`

To switch modes:
```bash
studyflow
# Navigate to: 👁️ Toggle Headless Mode
# Press Enter
```

### Managing Credentials

If you change your Canvas password:

```bash
studyflow
# Navigate to: 🔑 Reset Session Credentials
# Enter your new password
```

### Stopping StudyFlow

```bash
Ctrl + C
```

Safe to stop anytime. StudyFlow resumes exactly where it left off on the next run.

---

## Security & Privacy

**Your data stays on your computer.**

| Aspect | Details |
|--------|---------|
| **Credential Storage** | Saved locally in `~/.config/studyflow/`. Never uploaded to cloud services. |
| **Authentication** | Direct connection to your institution's Canvas server. No intermediaries. |
| **No Telemetry** | StudyFlow doesn't track usage, collect analytics, or phone home. |
| **No Cloud Sync** | Your credentials and data never leave your device. |
| **Local Logs Only** | Activity logs stored locally on your machine. |
| **Open Source** | Core code is publicly reviewable. No hidden backdoors or malware. |

---

## Source Availability

Parts of this project remain private to protect:
- Licensing infrastructure and key validation
- Backend authentication systems
- Service configuration and credentials
- Anti-abuse and fraud detection
- API keys and security mechanisms

**The npm package is fully public and functional.** You can install and use StudyFlow immediately. The private source code enables core infrastructure—the public package gives you everything you need.

---

## npm Package

**Package Name:** `studyflow-bot`  
**Registry:** [npm.js](https://www.npmjs.com/package/studyflow-bot)

```bash
# Install
npm install -g studyflow-bot

# Update to latest
npm install -g studyflow-bot@latest

# Uninstall
npm uninstall -g studyflow-bot
```

---

## CLI Commands

All commands are accessed through the interactive menu system. No flags or complex syntax needed.

```bash
# Start StudyFlow
studyflow

# From the menu, you can:
# • Start lecture management
# • View course list
# • Toggle headless/visible mode
# • Reset credentials
# • View settings
# • Exit
```

---

## Troubleshooting

**Q: How do I check if Node.js is installed?**  
A: Run `node --version` in your terminal. You should see a version number like `v18.0.0` or higher.

**Q: I get "command not found: studyflow"**  
A: Node.js or npm wasn't installed properly. Try:
- Windows: Close PowerShell and reopen it
- macOS/Linux: Close Terminal and reopen it
- Run `npm install -g studyflow-bot` again

**Q: StudyFlow crashed. How do I recover?**  
A: Just run `studyflow` again. It picks up exactly where it left off.

**Q: I see "Access Denied: Invalid license key"**  
A: Your license is invalid or expired. Contact your institution's administrator.

**Q: I changed my password. What now?**  
A: Launch StudyFlow and select `🔑 Reset Session Credentials`.

**Q: Can I use StudyFlow on multiple computers?**  
A: Yes. Each installation stores credentials locally on that computer.

**Q: Does StudyFlow work offline?**  
A: No. It needs an internet connection to authenticate and stream lectures.

**Q: What if my institution uses a different LMS?**  
A: StudyFlow currently supports Canvas only. Contact your administrator about other platforms.

**Q: My Mac says "app can't be opened because it's from an unidentified developer"**  
A: Right-click the file, click "Open," then click "Open" again in the popup.

**Q: Why is some code private?**  
A: See the [Source Availability](#source-availability) section above.

---

## Planned Improvements

We're working on:

📊 **Study Dashboard**  
Visual overview of lecture progress across all courses.

🧠 **Smarter Lecture Detection**  
Improved algorithms to identify and organize lectures.

🔍 **Diagnostics Command**  
Built-in troubleshooting tools for connection and setup issues.

🎨 **Better Terminal UI**  
Enhanced visual design and navigation.

📅 **Calendar Integrations**  
Sync lecture schedules with your calendar app.

---

## Disclaimer

**You are responsible for complying with your institution's Canvas LMS policies and academic integrity guidelines.**

StudyFlow is a productivity tool designed to help manage your lecture workflow. Use it responsibly and in accordance with your institution's policies. Misuse may result in account suspension or academic consequences.

**StudyFlow maintainers are not responsible for:**
- Policy violations at your institution
- Misuse of the tool
- Data loss or system issues
- Changes to Canvas LMS that break compatibility

Always review your institution's acceptable use policy before using any automation tools.

---

## Support & Links

📦 [npm Package](https://www.npmjs.com/package/studyflow-bot)  
🐙 [GitHub Repository](https://github.com/husky-696/StudyFlow)  
📚 [Canvas LMS Docs](https://community.canvaslms.com/)  
🔗 [Node.js](https://nodejs.org/)

---

<div align="center">

**Made for students who value their time.**

[npm](https://www.npmjs.com/package/studyflow-bot) • [GitHub](https://github.com/husky-696/StudyFlow)

</div>