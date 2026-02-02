# AWESOME DIGITAL FREEDOM

> **Status:** MAINTAINED  
> **Version:** 1.0.0 (Genesis)  
> **Philosophy:** The internet was built to be free. This repository restores that architecture.

## INTRODUCTION

This is not a list of "cool apps." This is a curated, high-level operational framework for reclaiming digital sovereignty. In an era of surveillance capitalism, algorithm-driven feeds, and walled gardens, `awesome-digital-freedom` serves as the toolkit for the user who refuses to be a product.

Everything listed here adheres to three core principles:
1.  **Open Source:** Verify, don't trust.
2.  **Privacy-Centric:** Data telemetry is stripped by default.
3.  **User Control:** You own the hardware; you should control the software.

---

## TABLE OF CONTENTS

1.  [Network Layer (DNS & Traffic Control)](#1-network-layer)
2.  [Browser Hardening (The Lens)](#2-browser-hardening)
3.  [Content Liberation (Media & Information)](#3-content-liberation)
4.  [Operating System Integrity (Debloat & Control)](#4-operating-system-integrity)
5.  [Privacy & Anonymity (Obfuscation)](#5-privacy--anonymity)

---

## 1. NETWORK LAYER

Control traffic before it enters your device. Blocking ads and trackers at the DNS level is more efficient than browser extensions.

*   **Pi-hole**  
    *Network-wide ad blocking via your own Linux hardware (Raspberry Pi/Docker).*  
    Acts as a DNS sinkhole. It intercepts DNS requests for known tracking domains and returns a null address.

*   **AdGuard Home**  
    *Network-wide software for blocking ads and tracking.*  
    Alternative to Pi-hole with support for DNS-over-HTTPS and DNS-over-TLS out of the box. Easier UI for management.

*   **NextDNS**  
    *Cloud-based firewall.*  
    If you cannot self-host, this provides blocklists, analytics, and parental controls without hardware requirements.

*   **Zapret / GreenTunnel**  
    *DPI (Deep Packet Inspection) Circumvention.*  
    Tools designed to bypass ISP-level censorship and throttling by fragmenting packets. Essential for accessing restricted protocols in heavy-surveillance regions.

---

## 2. BROWSER HARDENING

The browser is the primary attack vector. Default settings are unacceptable.

### BROWSERS
*   **LibreWolf**  
    A fork of Firefox that prioritizes privacy, security, and freedom. It removes telemetry, enables strict blocking, and disables anti-features like "Pocket" by default.

*   **Mullvad Browser**  
    Developed by the Tor Project and Mullvad VPN. Designed to minimize tracking and fingerprinting.

*   **Brave** (Configuration Required)  
    Usable for general purposes, but requires disabling "Brave Rewards," "Crypto Wallets," and "Sponsored Images" in settings to be truly clean.

### EXTENSIONS (THE ESSENTIAL STACK)
*   **uBlock Origin** (Raymond Hill)  
    *The only content blocker you need.*  
    *Configuration:* Enable "Advanced User" mode. Check all "Annoyance" filters. This is not just an adblocker; it is a wide-spectrum content blocker.

*   **Bypass Paywalls Clean**  
    *Information Access.*  
    A browser extension to bypass paywalls for recognized news sites. (Note: Use the GitLab repository for the unflagged version).

*   **LocalCDN**  
    Emulates Content Delivery Networks locally. Prevents you from pinging Google/Cloudflare servers just to load basic libraries like jQuery or Fonts.

---

## 3. CONTENT LIBERATION

Accessing media without algorithmic manipulation or paywalls.

### VIDEO & STREAMING
*   **NewPipe / Tubular** (Android)  
    Lightweight YouTube frontend. No Google account required, no ads, background play supported, and locally stored subscriptions.

*   **Grayjay**  
    A platform-agnostic media creator app. Allows following creators across YouTube, Twitch, Patreon, and Odysee in a single feed without algorithm interference.

*   **Piped / Invidious** (Web)  
    Alternative front-ends for YouTube. View content without feeding data to Google's tracking profile.

### AUDIO
*   **Spicetify**  
    Command-line tool to customize the official Spotify client. Supports custom themes, apps, and extensions to remove UI bloat.

*   **SpotX**  
    Modified Spotify client script that blocks audio ads and banner ads on the desktop version.

### KNOWLEDGE
*   **Anna's Archive**  
    The largest shadow library search engine. Aggregates data from Sci-Hub, Library Genesis, and Z-Library.

---

## 4. OPERATING SYSTEM INTEGRITY

Your OS should serve you, not the vendor.

*   **Chris Titus Tech's WinUtil**  
    *Windows Debloater.*  
    A PowerShell tool to strip Windows of telemetry, pre-installed "Candy Crush" bloatware, and unnecessary background services.
    ```powershell
    irm christitus.com/win | iex
    ```

*   **Revanced Manager** (Android)  
    Patcher for Android applications. Allows modification of APKs to remove ads, skip segments (SponsorBlock), and unlock background playback features.

*   **F-Droid**  
    FOSS (Free and Open Source Software) app store for Android. Replaces the Google Play Store for users who want verified, tracker-free applications.

---

## 5. PRIVACY & ANONYMITY

*   **Tor Project**  
    *The Onion Router.*  
    For true anonymity, not just privacy. Routes traffic through three layers of encryption.

*   **Veracrypt**  
    Open-source disk encryption software. Capable of creating hidden volumes (plausible deniability) within encrypted containers.

*   **Signal**  
    The gold standard for encrypted communication. Metadata minimization is the key feature here, unlike WhatsApp or Telegram (which are not E2E encrypted by default in groups).

---

> **⚠️DISCLAIMER:**  
> This repository is for educational and research purposes. The tools listed here are powerful. Users are responsible for adhering to their local laws and regulations regarding copyright and network usage.

> **MAINTAINED BY:**  
> root@cipher:~#
