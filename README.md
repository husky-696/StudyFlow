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
2. [🚀 Step-by-Step Installation Guides](#-step-by-step-installation-guides)
   - [🪟 Windows Guide](#-windows-guide)
   - [🍎 macOS Guide](#-macos-guide)
   - [🐧 Linux Guide](#-linux-guide)
3. [⚙️ First-Time Launch & Setup](#️-first-time-launch--setup)
4. [👁️ How to Toggle "Visible Browser Window" (Headed Mode)](#️-how-to-toggle-visible-browser-window-headed-mode)
5. [🛡️ Security & Privacy (Is my password safe?)](#️-security--privacy-is-my-password-safe)
6. [❓ Troubleshooting & FAQ](#-troubleshooting--faq)

---

## 🧩 Introduction

Watching and tracking dozens of video lectures every week on Canvas LMS can be tedious and time-consuming. 
**StudyFlow** is a smart, automatic helper that logs into your student portal, finds outstanding video lectures, and plays them sequentially to make sure your progress is completely logged.

- **No Coding Needed:** Operate everything using a simple interactive menu with your keyboard's arrow keys.
- **One-Click Sweep:** Automatically watch all unfinished videos across all your registered courses.
- **Privacy-First:** Your login password is saved only on your own computer. It is never sent to any third-party or administrator database.

---

## 🚀 Step-by-Step Installation Guides

To run StudyFlow, your computer needs a free background software called **Node.js** (which runs JavaScript programs). Follow these simple steps for your computer:

### 🪟 Windows Guide

1. **Download the Software:**
   - Go to the **[Official Node.js Website](https://nodejs.org/)**.
   - Click the big green button that says **"LTS"** (Long Term Support - recommended for most users) to download the installer.

2. **Install It:**
   - Double-click the downloaded file (`.msi`) and click "Next" through all prompts to install it with standard settings.

3. **Open the Command Window:**
   - Press the **Start** key on your keyboard or click the Windows icon in the bottom-left.
   - Search for **"PowerShell"** and click **"Windows PowerShell"** to open a blue/black window.

4. **Install StudyFlow:**
   - Copy this command, paste it into the PowerShell window (right-click or `Ctrl + V`), and press **Enter**:
     ```bash
     npm install -g studyflow-bot
     ```
   - *Wait a few seconds for the green loading progress bars to complete.*

5. **Run the Bot:**
   - Type **`studyflow`** in the window and press **Enter**!

---

### 🍎 macOS Guide

1. **Download the Software:**
   - Go to the **[Official Node.js Website](https://nodejs.org/)**.
   - Click the green **"LTS"** button to download the installer package.

2. **Install It:**
   - Double-click the downloaded `.pkg` file and follow the installer prompts to complete installation.

3. **Open the Terminal App:**
   - Press `Cmd + Space` on your Mac keyboard to open Spotlight Search.
   - Type **"Terminal"** and press **Enter** to open the command window.

4. **Install StudyFlow:**
   - Copy and paste this command into the Terminal, then press **Enter**:
     ```bash
     sudo npm install -g studyflow-bot
     ```
   - *Mac will ask for your computer's password to authorize the installation. Type your password and press **Enter**. Note: For security, no characters or stars will appear on screen while typing your password—just type it normally and press Enter!*

5. **Run the Bot:**
   - Type **`studyflow`** in the window and press **Enter**!

---

### 🐧 Linux Guide

For Linux environments, run these simple terminal commands to prepare Node.js and install StudyFlow globally:

1. **Install Node.js (Ubuntu/Debian):**
   ```bash
   sudo apt update
   sudo apt install -y nodejs npm
   ```

2. **Install StudyFlow globally:**
   ```bash
   sudo npm install -g studyflow-bot
   ```

3. **Run the Bot:**
   ```bash
   studyflow
   ```

---

## ⚙️ First-Time Launch & Setup

The first time you run `studyflow` in your terminal or PowerShell window, the onboarding assistant will ask for:

1. **Your License Key:**
   - Paste the unique activation key provided by your administrator (e.g. `00000000-xxxx-xxxx-xxxx-xxxxxxxxxxxx`) and press Enter.

2. **Your Student Credentials:**
   - **Canvas Student ID (Username):** Type your official student portal login ID and press Enter.
   - **Canvas Password:** Type your password and press Enter *(characters will not show up on screen while typing passwords for security)*.

3. **Automatic Browser Setup:**
   - If your computer doesn't have the necessary browser engine, the bot will automatically download Chromium on its first run.
   - If you see `No system browser detected. Installing companion browser...`, simply wait 1–2 minutes for the download to complete.

---

## 👁️ How to Toggle "Visible Browser Window" (Headed Mode)

By default, StudyFlow runs in **Headless mode**—meaning it works silently in the background without opening a browser window on your screen so you can keep working or studying.

If you want to watch the bot log in, click, and play the videos on your screen in real-time, you can toggle this whenever you want:

1. Launch **`studyflow`** in your command window.
2. Use the arrow keys on your keyboard to navigate to **`👁️ Toggle Headless Mode`** and press **Enter**.
3. A success alert will show **`HEADED (Visible Window)`**.
4. Now, when you choose an action to watch videos, a visible browser window will launch on your screen automatically so you can see the magic happen!
5. To hide the browser again, simply select the same menu option to toggle it back!

---

## 🛡️ Security & Privacy (Is my password safe?)

Entering your student portal ID and password in a terminal window can feel intimidating. StudyFlow was designed from day one to be 100% private, safe, and transparent:

- **Saved Completely Locally:** Your password and login credentials never leave your machine. They are saved securely in your private user configuration directory (`~/.config/studyflow/config.json`) on your own computer.
- **Direct Login Connections:** Your credentials are used exclusively to negotiate the login handshake directly with the official university Canvas LMS e-Class server (`canvas.bufs.ac.kr`). No data is ever sent to third parties, admin databases, or external APIs.
- **Fully Open Source:** Every single line of code in StudyFlow is open and reviewable by anyone, guaranteeing there are no backdoors, malware, or trackers inside the bot.

---

## ❓ Troubleshooting & FAQ

#### Q. How do I stop or force-quit the bot while it is running?
- Simply press the keys **`Ctrl` and `C`** at the same time (`Ctrl + C`) in your command window. This immediately and safely terminates the browser and exits the bot.

#### Q. I changed my university password! How do I update it?
- Choose the **`🔑 Reset Session Credentials`** option in the main interactive menu to safely clear and re-enter your student credentials.

#### Q. It says "Access Denied: Invalid or revoked license key".
- This means your license is invalid or has expired. Please contact your administrator to request a valid activation key.

#### Q. A video got stuck or timed out while loading.
- If your internet is slow or the university e-Class servers are busy, video loaders can occasionally timeout. Simply stop the bot (`Ctrl + C`) and run `studyflow` again to pick up exactly where you left off!

---

*Enjoy a smarter, fluid, and structured studying flow with StudyFlow CLI!*
