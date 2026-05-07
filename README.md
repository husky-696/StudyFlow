# ✦ StudyFlow CLI • Student Guide

<div align="center">
  <p align="center">
    <strong>✨ A beautiful, automated Canvas LMS lecture companion designed for students. ✨</strong>
  </p>
  <p align="center">
    <i>StudyFlow automatically plays and tracks your online e-Class lectures so you can focus on real studying, note-taking, and keeping your learning ledger 100% complete with zero manual clicking.</i>
  </p>
</div>

---

## 📖 Table of Contents

1. [🧩 Introduction](#-introduction)
2. [⭐ Key Features](#-key-features)
3. [📋 Prerequisites](#-prerequisites)
4. [🚀 Installation](#-installation)
   - [🪟 Windows](#-windows)
   - [🍎 macOS](#-macos)
   - [🐧 Linux](#-linux)
5. [⚙️ First-Time Setup](#️-first-time-setup)
6. [📖 Usage Guide](#-usage-guide)
   - [👁️ Headless Mode (Background) vs. Headed Mode (Visible)](#️-headless-mode-background-vs-headed-mode-visible)
   - [🔑 Managing Credentials](#-managing-credentials)
   - [⏹️ Stopping the Bot](#️-stopping-the-bot)
7. [🛡️ Security & Privacy](#️-security--privacy)
8. [❓ Troubleshooting & FAQ](#-troubleshooting--faq)
9. [📚 Additional Resources](#-additional-resources)

---

## 🧩 Introduction

Watching and tracking dozens of video lectures every week on Canvas LMS can be tedious and time-consuming. **StudyFlow** is a smart, automatic helper that:

- Logs into your student portal automatically
- Finds all outstanding video lectures across your courses
- Plays them sequentially in the background
- Tracks your progress to ensure your learning ledger stays 100% complete

All without requiring any manual clicking or coding knowledge!

---

## ⭐ Key Features

- **✅ No Coding Required:** Operate everything using a simple interactive menu with arrow keys
- **🎬 Automated Playback:** One-click sweep to watch all unfinished videos across all registered courses
- **🔒 Privacy-First:** Your login credentials stay only on your computer—never shared with third parties
- **🌙 Background Mode:** Run silently in the background while you work or study
- **👁️ Visible Mode:** Watch the bot work in real-time if you prefer
- **⚡ Automatic Browser Setup:** Downloads necessary browser engine on first run
- **🔐 Transparent & Open Source:** All code is reviewable; no backdoors or malware

---

## 📋 Prerequisites

Before installing StudyFlow, ensure you have:

- **Node.js** (v14 or higher) - A free runtime environment for JavaScript applications
- **Active Canvas LMS Account** - Your student credentials for your institution
- **License Key** - Provided by your administrator
- **Stable Internet Connection**

---

## 🚀 Installation

### 🪟 Windows

1. **Install Node.js:**
   - Visit the **[Official Node.js Website](https://nodejs.org/)**
   - Download the **LTS (Long Term Support)** version by clicking the green button
   - Double-click the `.msi` installer and follow the installation wizard
   - Click "Next" through all prompts to use default settings

2. **Open PowerShell:**
   - Press the **Windows** key on your keyboard
   - Search for **"PowerShell"** and open **"Windows PowerShell"**

3. **Install StudyFlow:**
   ```bash
   npm install -g studyflow-bot
   ```
   Wait for the installation to complete (you'll see green progress bars)

4. **Launch StudyFlow:**
   ```bash
   studyflow
   ```

---

### 🍎 macOS

1. **Install Node.js:**
   - Visit the **[Official Node.js Website](https://nodejs.org/)**
   - Download the **LTS** version for macOS
   - Open the `.pkg` installer and follow the setup wizard

2. **Open Terminal:**
   - Press `Cmd + Space` to open Spotlight Search
   - Type **"Terminal"** and press `Enter`

3. **Install StudyFlow:**
   ```bash
   sudo npm install -g studyflow-bot
   ```
   Your Mac will ask for your computer password (for security, no characters will appear while typing)

4. **Launch StudyFlow:**
   ```bash
   studyflow
   ```

---

### 🐧 Linux

1. **Install Node.js (Ubuntu/Debian):**
   ```bash
   sudo apt update
   sudo apt install -y nodejs npm
   ```

2. **Install StudyFlow:**
   ```bash
   sudo npm install -g studyflow-bot
   ```

3. **Launch StudyFlow:**
   ```bash
   studyflow
   ```

For other Linux distributions, refer to the **[Node.js official documentation](https://nodejs.org/en/download/package-manager/)**.

---

## ⚙️ First-Time Setup

When you run `studyflow` for the first time, the onboarding wizard will guide you through:

### 1. License Key Activation
- Paste your unique activation key provided by your administrator
- Format example: `00000000-xxxx-xxxx-xxxx-xxxxxxxxxxxx`
- Press `Enter` to confirm

### 2. Student Credentials
- **Canvas Student ID (Username):** Your official student portal login
- **Canvas Password:** Your password (characters won't display for security)
- These are saved locally on your computer only

### 3. Automatic Browser Setup
- StudyFlow automatically downloads **Chromium** (a browser engine) if needed
- This is a one-time download that takes 1–2 minutes
- You'll see: `No system browser detected. Installing companion browser...`
- Just wait for it to complete—the bot will then start normally

---

## 📖 Usage Guide

### 👁️ Headless Mode (Background) vs. Headed Mode (Visible)

By default, StudyFlow runs in **Headless mode** (silently in the background). You can toggle between modes:

#### Toggle to Visible Mode:
1. Launch `studyflow` in your command window
2. Navigate to **`👁️ Toggle Headless Mode`** using arrow keys
3. Press `Enter`
4. A success message will show **`HEADED (Visible Window)`**
5. The next time you start a video sweep, a browser window will open and you can watch the bot work in real-time

#### Toggle Back to Headless:
- Select the same menu option again to hide the browser window

**Tip:** Use visible mode for troubleshooting or to see the bot in action; use headless mode when you want to work uninterrupted.

---

### 🔑 Managing Credentials

#### Update Your Password:
If you've changed your university password:
1. Launch `studyflow`
2. Navigate to **`🔑 Reset Session Credentials`**
3. Re-enter your new credentials
4. Your updated information will be saved securely

---

### ⏹️ Stopping the Bot

To stop StudyFlow at any time:
```bash
Ctrl + C
```
This immediately and safely terminates the browser and exits the bot. You can resume exactly where you left off on your next run.

---

## 🛡️ Security & Privacy

**Is my password safe?**

Yes. StudyFlow was designed from the ground up with security and privacy as core principles:

| Aspect | How It Works |
|--------|-------------|
| **Local Storage** | Your password and credentials are saved **only** on your computer in `~/.config/studyflow/config.json`. They never leave your machine. |
| **Direct Authentication** | Your credentials communicate directly with your official university Canvas LMS server (`canvas.bufs.ac.kr`). No StudyFlow servers are involved. |
| **Open Source** | Every line of code is publicly available and reviewable. There are no hidden backdoors, malware, or trackers. |
| **No Cloud Sync** | Your data is never uploaded, backed up, or shared with any cloud services or third parties. |
| **Transparent Logging** | The bot logs its actions locally; logs are also kept only on your computer. |

---

## ❓ Troubleshooting & FAQ

#### Q: How do I check if Node.js is installed?
**A:**
```bash
node --version
npm --version
```

#### Q: How do I uninstall StudyFlow?
**A:**
```bash
npm uninstall -g studyflow-bot
```

#### Q: StudyFlow crashes or exits unexpectedly. What should I do?
**A:** 
- Check your internet connection
- Try running `studyflow` again—the bot will resume from where it stopped
- If the problem persists, see the video loading issue below

#### Q: A video got stuck or timed out while loading.
**A:** If your internet is slow or the university e-Class servers are busy, video loaders can timeout. Simply:
1. Stop the bot: `Ctrl + C`
2. Run `studyflow` again
3. The bot will resume exactly where it left off

#### Q: It says "Access Denied: Invalid or revoked license key".
**A:** Your license is invalid or has expired. Contact your administrator to request a valid activation key.

#### Q: I changed my university password. How do I update it?
**A:** 
1. Launch `studyflow`
2. Choose **`🔑 Reset Session Credentials`** from the menu
3. Re-enter your new password

#### Q: Can I run StudyFlow on multiple computers?
**A:** Yes, but use different license keys for each computer if your administrator provides them. Each installation stores credentials locally on that computer only.

#### Q: What if my institution uses a different LMS (not Canvas)?
**A:** StudyFlow is currently designed for Canvas LMS. Contact your administrator about compatibility with other platforms.

#### Q: Does StudyFlow work offline?
**A:** No, StudyFlow requires a stable internet connection to authenticate and stream lectures from your university's servers.

---

## 📚 Additional Resources

- **[Node.js Official Website](https://nodejs.org/)** – Download and learn about Node.js
- **[Canvas LMS Documentation](https://community.canvaslms.com/)** – Information about Canvas
- **[GitHub Repository](https://github.com/husky-696/StudyFlow)** – Source code and issue tracking

---

## 💡 Tips for Best Results

1. **Run During Off-Peak Hours:** Run StudyFlow during times when your university's servers are less busy (late evening or early morning)
2. **Stable Connection:** Ensure your internet connection is stable before starting a large video sweep
3. **Keep Headless On:** Use headless mode (default) to avoid distractions while working
4. **Regular Updates:** Periodically update StudyFlow to get bug fixes and improvements:
   ```bash
   npm install -g studyflow-bot@latest
   ```

---

*Made with ❤️ for students who want to focus on learning, not logistics.*

**Enjoy a smarter, fluid, and structured studying flow with StudyFlow CLI!** 🚀
