<div align="center">
  <img width="735" height="459" alt="Linux Logo" src="https://github.com/user-attachments/assets/94c53e80-2d48-4d53-8bad-b6473e1cfd9b" />

  <h1 style="border-bottom: none; margin-bottom: 0;">Daily Linux</h1>
  <p>A complete, step-by-step guide to setting up, understanding, and making Linux your daily driver.</p>

  <br>

  <!-- Bright Modern Badges -->
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-007EC6?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="License: MIT"></a>
  <img src="https://img.shields.io/badge/Platform-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Platform: Linux">
  <img src="https://img.shields.io/badge/Status-Active-2EA043?style=for-the-badge&logo=checkmarx&logoColor=white" alt="Status: Active">
</div>

<br><br>

## Index

> *The complete roadmap will be built here as chapters are added.*

---

## Overview

Welcome to **Daily Linux**. 

Most Linux documentation either treats you like a seasoned server administrator or hands you a list of terminal commands to copy and paste without explaining *why*. This repository is built differently. 

It is designed to be a practical, no-nonsense companion for transitioning to Linux and actually using it as your primary daily driver. Whether you are dual-booting for the first time, reviving an old machine, or completely ditching Windows/macOS, this guide focuses on real-world usability. 

**The goal is simple:** Help you break down system configurations, comfortably navigate the terminal, manually fix things when they go wrong, and tailor your desktop environment to fit your exact workflow.

---

## Introduction

### 🐧 What exactly is Linux?
Think of an operating system like a car. Windows and macOS are fully built vehicles—you get them as-is, with the dashboard, seats, and paint job already chosen for you by the manufacturer. 

**Linux**, strictly speaking, is just the *engine* (the kernel). It is the invisible core software that lets your computer's hardware talk to your applications. Because this engine is open-source, anyone is free to take it and build their own custom vehicle around it.

### 📦 What is a "Distro"?
Since you can't drive a car that is just an engine, developers bundle the Linux kernel with a graphical interface, a file manager, settings menus, and pre-installed apps to give you a complete, ready-to-use operating system. 

This complete package is called a **Linux Distribution** (or "Distro" for short). 
*(Examples: Ubuntu, Linux Mint, Fedora, Pop!_OS).*

### 🧬 The Different Linux Families
While there are hundreds of distros out there, most are not built from scratch. They are usually customized variations based on a few major "parent" families. The biggest difference between these families is **how they install software** and **how often they get system updates**.

<br>

<table>
  <tr>
    <td align="center" width="10%"><img src="https://skillicons.dev/icons?i=debian" width="60" alt="Debian" /></td>
    <td><b>Debian-based (e.g., Ubuntu, Linux Mint, Pop!_OS)</b><br>The most popular and beginner-friendly family. They prioritize extreme stability. Software is heavily tested before it reaches you, making the system highly reliable. <i>(Uses the <code>apt</code> package manager)</i>.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://skillicons.dev/icons?i=arch" width="60" alt="Arch" /></td>
    <td><b>Arch-based (e.g., Arch Linux, Manjaro, EndeavourOS)</b><br>Built for users who want the absolute newest software the exact second it is released (known as a "rolling release"). Offers ultimate, lightweight control. <i>(Uses the <code>pacman</code> package manager)</i>.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://skillicons.dev/icons?i=redhat" width="60" alt="Red Hat" /></td>
    <td><b>Red Hat-based (e.g., Fedora, Rocky Linux)</b><br>The sweet spot in the middle. Very popular with developers and in enterprise environments, offering highly up-to-date features with a rock-solid foundation. <i>(Uses the <code>dnf</code> package manager)</i>.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/opensuse/opensuse-original.svg" width="60" alt="SUSE" /></td>
    <td><b>SUSE-based (e.g., openSUSE)</b><br>A massive, independent parent base highly respected in enterprise and European markets. Known for its incredibly powerful system configuration tool called YaST. <i>(Uses the <code>zypper</code> package manager)</i>.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nixos/nixos-original.svg" width="60" alt="NixOS" /></td>
    <td><b>Independents & Source-based (e.g., NixOS, Gentoo, Alpine)</b><br>Distros built completely from scratch with their own unique rules. Ranges from declarative systems where the whole OS is built from one text file (NixOS), to systems where you compile every app from raw source code (Gentoo).</td>
  </tr>
</table>

> **Note:** While the Linux ecosystem contains dozens of other niche and independent bases, the families listed above power **99%** of what you will actually encounter and use as a daily driver.

<br>

### 🛒 Wait, what is a "Package Manager"?

In the table above, you probably noticed weird commands like `apt`, `pacman`, or `dnf` being called package managers. If you are coming from Windows or macOS, you might be wondering what exactly that means.

Think of a package manager as the **ultimate, super-charged App Store** for your entire computer. 

Normally, installing a program means opening a web browser, searching for the software, dodging fake download buttons, downloading a bulky installer file (`.exe` or `.dmg`), clicking "Next" five times, and then hoping the app remembers to update itself later. 

Linux does not work like that. All verified, safe software is stored in a massive central library (called a *repository*). Your package manager is essentially your personal shopper. You just tell it what you want, and it goes to the library, finds the app, grabs any other background files the app needs to run (called *dependencies*), and installs it perfectly.

Want Firefox? You don't open a browser. You just open your terminal and tell your package manager to go get it:

*   **On Debian/Ubuntu:** `sudo apt install firefox`
*   **On Arch:** `sudo pacman -S firefox`

Press Enter, and boom—it is installed in seconds. 

The absolute best part? When it is time to update your computer, you don't have to update your apps one by one. The package manager updates your core operating system **and** every single app you have installed all at the exact same time.
