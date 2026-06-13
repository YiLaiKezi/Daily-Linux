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

<br>

## 📌 Table of Contents

<br>

<table width="100%">
  <tr>
    <th align="center" width="10%">ID</th>
    <th align="left">Section Topic</th>
  </tr>
  <tr>
    <td align="center"><code>1.0</code></td>
    <td><b><a href="#10-overview">Overview</a></b></td>
  </tr>
  <tr>
    <td align="center"><code>2.0</code></td>
    <td><b><a href="#20-introduction">Introduction</a></b></td>
  </tr>
  <tr>
    <td align="center"><code>2.1</code></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp; ↳ <a href="#21--what-exactly-is-linux">What exactly is Linux?</a></td>
  </tr>
  <tr>
    <td align="center"><code>2.2</code></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp; ↳ <a href="#22--what-is-a-distro">What is a "Distro"?</a></td>
  </tr>
  <tr>
    <td align="center"><code>2.3</code></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp; ↳ <a href="#23--the-different-linux-families">The Different Linux Families</a></td>
  </tr>
  <tr>
    <td align="center"><code>2.4</code></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp; ↳ <a href="#24--wait-what-is-a-package-manager">Wait, what is a "Package Manager"?</a></td>
  </tr>
  <tr>
    <td align="center"><code>2.5</code></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp; ↳ <a href="#25-️-what-is-a-desktop-environment-de">What is a "Desktop Environment" (DE)?</a></td>
  </tr>
  <tr>
    <td align="center"><code>2.6</code></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp; ↳ <a href="#26--popular--actively-maintained-des">Popular & Actively Maintained DEs</a></td>
  </tr>
  <tr>
    <td align="center"><code>2.7</code></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp; ↳ <a href="#27-️-special-category-tiling-window-managers-twms">Tiling Window Managers (TWMs)</a></td>
  </tr>
  <tr>
    <td align="center"><code>3.0</code></td>
    <td><b><a href="#30--visual-tour-exploring-the-environments">Visual Tour: Exploring the Environments</a></b></td>
  </tr>
  <tr>
    <td align="center"><code>3.1</code></td>
    <td>&nbsp;&nbsp;&nbsp;&nbsp; ↳ <a href="#31--gnome">GNOME</a></td>
  </tr>
</table>

<br>

## 1.0 Overview

Welcome to **Daily Linux**. 

Most Linux documentation either treats you like a seasoned server administrator or hands you a list of terminal commands to copy and paste without explaining *why*. This repository is built differently. 

It is designed to be a practical, no-nonsense companion for transitioning to Linux and actually using it as your primary daily driver. Whether you are dual-booting for the first time, reviving an old machine, or completely ditching Windows/macOS, this guide focuses on real-world usability. 

**The goal is simple:** Help you break down system configurations, comfortably navigate the terminal, manually fix things when they go wrong, and tailor your desktop environment to fit your exact workflow.

---

## 2.0 Introduction

### 2.1 🐧 What exactly is Linux?
Think of an operating system like a car. Windows and macOS are fully built vehicles—you get them as-is, with the dashboard, seats, and paint job already chosen for you by the manufacturer. 

**Linux**, strictly speaking, is just the *engine* (the kernel). It is the invisible core software that lets your computer's hardware talk to your applications. Because this engine is open-source, anyone is free to take it and build their own custom vehicle around it.

### 2.2 📦 What is a "Distro"?
Since you can't drive a car that is just an engine, developers bundle the Linux kernel with a graphical interface, a file manager, settings menus, and pre-installed apps to give you a complete, ready-to-use operating system. 

This complete package is called a **Linux Distribution** (or "Distro" for short). 
*(Examples: Ubuntu, Linux Mint, Fedora, Pop!_OS).*

### 2.3 🧬 The Different Linux Families
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

### 2.4 🛒 Wait, what is a "Package Manager"?

In the table above, you probably noticed weird commands like `apt`, `pacman`, or `dnf` being called package managers. If you are coming from Windows or macOS, you might be wondering what exactly that means.

Think of a package manager as the **ultimate, super-charged App Store** for your entire computer. 

Normally, installing a program means opening a web browser, searching for the software, dodging fake download buttons, downloading a bulky installer file (`.exe` or `.dmg`), clicking "Next" five times, and then hoping the app remembers to update itself later. 

Linux does not work like that. All verified, safe software is stored in a massive central library (called a *repository*). Your package manager is essentially your personal shopper. You just tell it what you want, and it goes to the library, finds the app, grabs any other background files the app needs to run (called *dependencies*), and installs it perfectly.

Want Firefox? You don't open a browser. You just open your terminal and tell your package manager to go get it:

*   **On Debian/Ubuntu:** `sudo apt install firefox`
*   **On Arch:** `sudo pacman -S firefox`

Press Enter, and boom—it is installed in seconds. 

The absolute best part? When it is time to update your computer, you don't have to update your apps one by one. The package manager updates your core operating system **and** every single app you have installed all at the exact same time.

<br>

### 2.5 🖥️ What is a "Desktop Environment" (DE)?

If the Linux kernel is the car's engine, the **Desktop Environment (DE)** is the dashboard, the steering wheel, the seats, and the paint job. 

On Windows or macOS, you are completely stuck with the interface Microsoft or Apple gives you. The visual layout is permanently glued to the operating system. If you don't like the Windows Start Menu or the Mac Dock, you just have to deal with it. 

Linux treats the visual interface as just another piece of software. You can completely rip it out, swap it for something else, or customize it entirely without ever breaking the underlying operating system. Because of this, Linux distributions often come in different "flavors." A flavor is simply the exact same core OS, but shipped with a different visual interface built on top.

### 2.6 ✨ Popular & Actively Maintained DEs

While there are dozens of interfaces out there, these are the heavyweights that are highly polished, well-funded, and actively updated today:

<br>

<table>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/gnome/4A86CF" width="60" alt="GNOME" /></td>
    <td><b>GNOME</b><br>Extremely modern and minimalist. It heavily focuses on workspaces, trackpad gestures, and keyboard navigation. It feels like a premium mix between macOS and a tablet interface. <i>(Default on Ubuntu and Fedora)</i>.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/kde/1D99F3" width="60" alt="KDE Plasma" /></td>
    <td><b>KDE Plasma</b><br>The customizer's absolute dream. Out of the box, it feels very traditional (similar to Windows), but it allows you to tweak absolutely every single pixel, color, and animation to your exact liking.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/linuxmint/87A556" width="60" alt="Cinnamon" /></td>
    <td><b>Cinnamon</b><br>Designed from the ground up to be the most comfortable, seamless, and rock-solid transition for a lifelong Windows user. Familiar, straightforward, and stays completely out of your way. <i>(Default on Linux Mint)</i>.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/xfce/2284F2" width="60" alt="XFCE" /></td>
    <td><b>XFCE</b><br>The lightweight champion. A fast, traditional interface designed to use incredibly low system memory and battery, making it perfect for reviving old hardware or keeping your system ridiculously snappy.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://raw.githubusercontent.com/mate-desktop/mate-desktop.org/master/files/mate.svg" width="60" alt="MATE" /></td>
    <td><b>MATE</b><br>The classic workhorse. Built as a direct continuation of older, traditional Linux interfaces. It is extremely stable, highly reliable, and ignores flashy trends in favor of getting work done.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/solus/5294E2" width="60" alt="Budgie" /></td>
    <td><b>Budgie</b><br>A sleek, modern interface built completely from scratch. It perfectly balances a beautiful, elegant look with user-friendly controls without being overly heavy on your computer's resources.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/elementary/64BAED" width="60" alt="Pantheon" /></td>
    <td><b>Pantheon</b><br>Hyper-focused on clean typography, smooth animations, and a strict, distraction-free aesthetic. If you want a beautifully curated, macOS-like experience out of the box, this is it. <i>(Default on elementary OS)</i>.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/lubuntu/0068C8" width="60" alt="LXQt" /></td>
    <td><b>LXQt</b><br>The absolute featherweight. Even lighter than XFCE in many cases, designed purely to make ancient laptops or highly constrained hardware run smoothly without sacrificing a graphical interface.</td>
  </tr>
</table>

<br>

### 2.7 🛠️ Special Category: Tiling Window Managers (TWMs)

Not everyone wants a full "desktop environment." Power users who want absolute maximum speed often use **Window Managers**. Instead of windows floating around and overlapping like on Windows or Mac, a Tiling Window Manager automatically snaps every window perfectly to the screen in a grid. You never use a mouse to drag or resize—everything is done instantly with keyboard shortcuts.

<br>

<table>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/hyprland/00A489" width="60" alt="Hyprland" /></td>
    <td><b>Hyprland</b><br>The current absolute superstar of the Linux customization scene. It brings tiling window managers into the modern age with incredibly smooth, buttery animations, blur effects, and rounded corners, all while being incredibly fast. <i>(Runs on modern Wayland)</i>.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/sway/E95420" width="60" alt="Sway" /></td>
    <td><b>Sway</b><br>A highly efficient, modern tiling manager built as the drop-in replacement for old-school setups. Clean, fast, native Wayland support, and fully keyboard-driven.</td>
  </tr>
  <tr>
    <td align="center" width="10%"><img src="https://cdn.simpleicons.org/i3/4C7A99" width="60" alt="i3wm" /></td>
    <td><b>i3wm</b><br>The timeless classic workhorse of window management. It is lightweight, rock-solid, and runs on the older X11 server environment, using practically zero system resources.</td>
  </tr>
</table>

> **Note:** While the broader Linux community offers endless customization options, the environments listed above represent the most stable, heavily maintained, and reliable interfaces to pick from for a bulletproof daily driver workflow.
> 
<br>

## 3.0 📸 Visual Tour: Exploring the Environments

While reading about different desktop environments gives you a solid foundation, seeing them in action makes all the difference. Your interface is where you will spend all of your time on the computer, so finding a layout that feels intuitive and comfortable for your daily workflow is essential. 

Below, we will take a visual look into each of these major environments, breaking down their unique designs alongside the specific **Pros and Cons** they offer to help you 
choose the perfect daily driver.

---

## 3.1 <img src="https://cdn.simpleicons.org/gnome/4A86CF" width="35" align="top" alt="GNOME Logo"> GNOME

<p>
  <b>🌟 The "Apple" of the Linux World</b><br>
  GNOME is sleek, highly polished, and incredibly opinionated. If you are looking for a traditional Windows-style Start menu, turn back now. GNOME completely ditches the classic desktop layout in favor of a modern, distraction-free "Activities Overview". It is built for people who love using keyboard shortcuts and buttery-smooth trackpad gestures to zip between workspaces. You either love its workflow, or you hate it—there is almost no in-between.
</p>

<br>

<div align="center">
  <img src="https://github.com/user-attachments/assets/c5c1a564-e4af-45a0-ad59-4cec9d482ec3" width="100%" alt="GNOME Desktop View">
  <br><br>
  <img src="https://github.com/user-attachments/assets/853ba973-744e-4e91-9048-3196919e77e6" width="100%" alt="GNOME Activities View">
  <br><br>
  <img src="https://github.com/user-attachments/assets/d8e4806a-858c-4845-8229-e947197cfef3" width="100%" alt="GNOME App Grid View">
</div>

<br>

<table>
  <tr>
    <td width="50%" valign="top">
      <h3 align="center">✨ The Good Stuff</h3>
      <hr>
      <b>🚀 Keyboard Ninja Workflow</b><br>
      Once you learn the shortcuts, flying through workspaces, searching for files, and launching apps feels ridiculously fast and fluid.<br><br>
      <b>🖐️ Trackpad Magic</b><br>
      If you are on a laptop, GNOME features the absolute best 1:1 swipe gestures in the Linux world. It feels incredibly premium and responsive.<br><br>
      <b>📦 Incredible App Ecosystem</b><br>
      It comes with a fantastic suite of beautifully designed, native apps out of the box (like Nautilus for files) that all share the exact same clean aesthetic.<br><br>
      <b>🎨 Next-Level Aesthetics</b><br>
      While it looks solid stock, it becomes dynamic and gorgeous when you tap into community extensions. Plugins like <i>Blur my Shell</i> add glassmorphism and stunning blur effects that make the UI look incredibly modern.
    </td>
    <td width="50%" valign="top">
      <h3 align="center">⚠️ The Harsh Truth</h3>
      <hr>
      <b>🍔 Heavier Resource Usage</b><br>
      It is a heavy hitter. It uses noticeably more background memory and CPU than lighter desktops, making it less ideal for ancient hardware.<br><br>
      <b>🧱 "My Way or the Highway"</b><br>
      Pure GNOME hides the minimize button and desktop icons to force you into using workspaces. <i>(Note: Ubuntu adds them back, but on Fedora/Arch, you need to install a "Tweaks" app to get them).</i><br><br>
      <b>🧩 Extension Roulette</b><br>
      Those awesome aesthetics come with a catch. Because extensions inject code directly into the shell, major GNOME system updates will frequently break your favorite blur plugins until developers patch them.
    </td>
  </tr>
</table>

<p align="center">
  <b>🎯 Best For:</b> Minimalists, keyboard ninjas, and anyone looking for a highly polished, premium interface out of the box.<br>
  🔗 <b>More Info:</b> <a href="https://www.gnome.org/">gnome.org</a>
</p>

<br>
