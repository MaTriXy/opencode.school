---
title: "Prerequisites"
slug: prerequisites
description: "What you need before getting started with OpenCode."
order: 1
---

Before we install anything, let's make sure your computer is ready.

## A computer

OpenCode Desktop runs on **macOS**, **Windows**, and **Linux**. Any modern computer from the last 5-6 years should work fine. There are no special hardware requirements — the AI models run in the cloud, not on your machine.

You need:

- A reliable internet connection
- At least 500 MB of free disk space
- A reasonably up-to-date operating system

## Check your system

Here's how to find out what you're working with:

**macOS** — Click the Apple menu () in the top-left corner of your screen, then click "About This Mac." You'll see your chip (Apple M1/M2/M3/M4 or Intel), how much memory (RAM) you have, and which version of macOS you're running. macOS 12 (Monterey) or later is recommended.

**Windows** — Press `Windows + I` to open Settings, then go to System > About. Look for your Processor, Installed RAM, and Windows edition. Windows 10 (version 1903 or later) or Windows 11 is required.

**Linux** — Open a terminal and run `uname -a` to see your kernel version. Most recent distributions work well — Ubuntu 20.04+, Fedora 36+, Debian 11+, and Arch Linux are all supported.

## Windows users: we recommend WSL

If you're on Windows, we recommend installing **Windows Subsystem for Linux (WSL)**.

WSL lets you run a full Linux environment directly inside Windows. It's free, built into Windows 10 and 11, and takes just one command to install. Open PowerShell as Administrator and run:

```
wsl --install
```

After installation, restart your computer and you'll have a Linux terminal available alongside your regular Windows desktop.

**Why WSL?** Many developer tools — including parts of OpenCode — work more smoothly in a Linux environment. WSL gives you the best of both worlds. The OpenCode Desktop app runs natively on Windows regardless, but if you later want to use the terminal interface or advanced features, having WSL will make your life easier.

Some lessons in this course reference terminal commands that assume a Unix-like shell (macOS, Linux, or WSL). If you're on Windows without WSL, you may need to adapt those commands for PowerShell.

For more details, see [Microsoft's WSL installation guide](https://learn.microsoft.com/en-us/windows/wsl/install) and OpenCode's [Windows (WSL) documentation](https://opencode.ai/docs/windows-wsl).

## A text editor

You'll need a text editor for viewing and editing configuration files. We recommend [Visual Studio Code](https://code.visualstudio.com/) — it's free, works on all platforms, and has great support for the JSON/JSONC files that OpenCode uses for configuration.

If you don't want to install anything extra, you can use the text editor that comes with your computer:

- **macOS**: TextEdit (in your Applications folder). Go to TextEdit > Settings and select "Plain Text" as the default format — otherwise it will try to save files as rich text.
- **Windows**: Notepad (search for it in the Start menu).
- **Linux**: Varies by distribution — gedit (GNOME), Kate (KDE), mousepad (XFCE), or `nano` in the terminal.

OpenCode itself will handle most file creation and editing. The text editor is mainly for when you want to manually inspect or tweak [config](/glossary#config) files.

## That's it

No special software to install yet, no accounts to create. If you have a computer with an internet connection and a text editor, you're ready for the next lesson.
