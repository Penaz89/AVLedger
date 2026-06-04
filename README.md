<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="internal/assets/AVLedger-wordmark-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="internal/assets/AVLedger-wordmark-light.svg">
    <img alt="AVLedger Logo" src="internal/assets/AVLedger-wordmark-light.svg" width="450">
  </picture>

  <br />
  <br />

  **The minimalist, open-source, EASA-compliant digital logbook for Aircraft Maintenance Engineers (AME).**<br />
  *Made by engineers, for engineers.*

  <br />

  [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?style=for-the-badge)](https://www.gnu.org/licenses/gpl-3.0)
  [![Go Version](https://img.shields.io/github/go-mod/go-version/Pnz89/AVLedger?color=00add8&style=for-the-badge)](https://golang.org/)
  [![GitHub Release](https://img.shields.io/github/v/release/Pnz89/AVLedger?style=for-the-badge)](https://github.com/Pnz89/AVLedger/releases)
</div>

---

## ⚡ Why AVLedger?

Aircraft Maintenance Engineers don't have time for bloated interfaces, sluggish exports, or complex subscription models. **AVLedger** gets out of the way and does exactly what it says:

- 🔧 **Track maintenance tasks** — Record every job done on every aircraft, clearly and quickly.
- 📄 **Export to PDF in seconds** — Because paperwork should never be the bottleneck.
- 💾 **Own your data** — SQLite means your data is always one file away from safe. Zero subscriptions required. Total freedom. Absolute privacy.

---

## ✨ Features

### Core Logging & Management
- **Task Logging:** Efficiently record maintenance work with precise tracking for Task Duration, ATA Chapters, Job Types, and Workorders.
- **Aircraft Management:** Build and manage a centralized list of aircraft (Type, Registration). Select aircraft directly from dropdowns to ensure data consistency.
- **Assessor Management:** Store and organize Assessor details (Name, License, Company Approval). Quickly link them to tasks and automatically expand their full details during PDF export.

### Smart Sync & Multi-User
- **Multi-User Profiles:** Perfect for shared computers. Create personal profiles, switch between them instantly, and save individual databases locally.
- **Smart Cloud Backup:** Automatically detects cloud sync folders (Dropbox, Google Drive, OneDrive, Nextcloud, ownCloud, pCloudDrive, Apple iCloud) to generate **secure automatic backups** whenever the app is closed. If a newer backup from another PC is detected upon startup, AVLedger will safely prompt you to import it.
- **Hot-Swappable DB:** Full manual control. Connect to or switch between any local/remote SQLite database files instantly from the UI without restarting.

### Performance & UI
- **Advanced Filtering:** Instantly narrow down your maintenance history by Aircraft, Category, ATA Chapter, or Job Type.
- **Lightning-Fast PDF Export:** Generate beautifully styled, ready-to-print PDF logbooks seamlessly. Optimized for black-and-white printing with smart text wrapping.
- **Refined Aesthetics:** A modern, minimal Fyne-based interface featuring custom themes (Light/Dark), freely resizable auxiliary windows, zebra-striped tables, and clear visual hierarchy.
- **Ultra Lightweight:** Minimal footprint, standalone binaries, and no heavy unnecessary dependencies. Completely Free and Open-Source Software (FOSS).

---

## 🧠 Philosophy: Keep It Simple, Stupid (KISS)

AVLedger is built around the fundamental **KISS** principle. 

No locked-in cloud SaaS. No subscriptions. No unnecessary complexity. Just a tool that works smoothly on your machine, under your control. If a feature doesn't help an AME log a task faster or export cleaner, it doesn't belong in AVLedger.

---

## 🚀 Getting Started

### Prerequisites

- [Go](https://golang.org/dl/) 1.21 or later

### Build from source

#### 🐧 Linux, 🍏 macOS, 😈 FreeBSD

```bash
git clone https://github.com/Penaz89/avledger.git
cd avledger
go build -o avledger .

# Run the app
./avledger
```

#### 🪟 Windows

```powershell
git clone https://github.com/Penaz89/avledger.git
cd avledger
go build -o avledger.exe .

# Run the app
.\avledger.exe
```

---

## 🛠 Tech Stack

Built with modern, reliable technologies:

- **Language:** [Go](https://golang.org/)
- **UI Framework:** [Fyne](https://fyne.io/)
- **Database:** [SQLite](https://www.sqlite.org/) — single file, zero setup, easy backup
- **PDF Generation:** [go-pdf/fpdf](https://github.com/go-pdf/fpdf)

---

## 🤝 Contributing

Contributions are always welcome! Please keep the KISS philosophy in mind — if a feature adds complexity without clear value, it probably doesn't belong here.

1. **Fork** the repo
2. **Create** your branch (`git checkout -b feature/your-feature`)
3. **Commit** your changes (`git commit -m 'Add some feature'`)
4. **Push** to the branch (`git push origin feature/your-feature`)
5. **Open** a Pull Request

---

## 📜 License

AVLedger is open-source and licensed under the **[GNU General Public License v3.0](./LICENSE)**.

You are free to use, study, modify, and distribute this software, provided that any derivative work is also distributed under the same license.

<br />
<div align="center">
  <i>The logbook that belongs to you.</i>
</div>
