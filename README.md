# MemoryOS — Beta

Local-first macOS storage intelligence. Scans your Mac, classifies storage usage, finds duplicate files, surfaces cleanup recommendations, and includes an AI assistant that understands your entire Mac.

**MemoryOS never deletes files automatically.**

---

## Download

[**Download MemoryOS v0.1.0 for macOS (Apple Silicon)**](https://github.com/tanmayjha1/memoryos-releases/releases/latest)

---

## Install

1. Download `MemoryOS_0.1.0_aarch64.dmg`
2. Open the DMG — **right-click → Open** (not double-click) to bypass the macOS security warning
3. Drag **MemoryOS** into your Applications folder
4. Launch from Applications or Spotlight

> **"Apple cannot check it for malicious software"** — expected for an unsigned app. Right-click → Open bypasses this.

> **"MemoryOS is damaged and can't be opened"** — macOS quarantined the file during download. Run this in Terminal, then try again:
> ```
> xattr -c ~/Downloads/MemoryOS_0.1.0_aarch64.dmg
> ```

---

## How to Use

### 1. Scan a folder
Type a folder path in the top bar or click **Browse** to pick one with Finder. Hit **Analyze**. Start with your home folder (`/Users/yourname`) for the full picture. Large folders take a moment — the scan runs in the background.

### 2. Dashboard
Overview of your scan: total files, duplicate groups, recommendation count, and a storage breakdown by category (Documents, Media, Developer files, etc.).

### 3. Folders
Shows the largest files and subdirectories inside your scanned folder, so you can find what's eating the most space.

### 4. Duplicates
Lists every group of identical files found in your scan, grouped by wasted space. Trash individual files — they go to Trash, not permanent delete.

### 5. Recommendations
Cleanup suggestions with a risk level for each item (Safe / Review / Caution).

### 6. System Data
Shows apps you haven't opened in 30+ days, and APFS Time Machine local snapshots that can be safely removed.

### 7. Ask AI
Ask anything about your storage in plain English:
- *"What's taking up the most space?"*
- *"Do I have large video files in Downloads?"*
- *"Where are my iPhone backups?"*
- *"Is it safe to delete Xcode DerivedData?"*

The AI can search file contents (PDFs, Word docs, PowerPoints) and knows common Mac locations like Docker images, npm cache, and Xcode build artifacts.

---

## Privacy

- Runs entirely on your Mac — no account, no cloud sync
- Scan data stored locally in `~/Library/Application Support/MemoryOS/`
- AI responses use OpenAI — only category totals and folder sizes are sent, never file paths or file contents

---

## Feedback

This is a beta — bugs and rough edges are expected. If something breaks or feels off, reach out directly with:
- What you were doing
- What happened vs. what you expected
- Your macOS version (Apple menu → About This Mac)

Thanks for testing!
