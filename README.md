# MemoryOS

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

> **"Apple cannot check it for malicious software"** — this is expected. The app is not yet notarized. Right-click → Open bypasses this warning.

---

## How to Use

### 1. Scan a folder
Type a folder path in the top bar or click **Browse**. Start with your home folder (`/Users/yourname`) for the full picture.

### 2. Dashboard
- Storage breakdown by category
- Largest folders
- Duplicate files grouped by wasted space
- Cleanup recommendations with risk levels (Safe / Review / Caution)

### 3. Duplicates
Lists every group of identical files. Trash individual files — sent to Trash, not permanent delete.

### 4. System Data
Shows `~/Library` usage: caches, logs, containers, app support, Messages attachments, apps unused for over a year.

### 5. AI Chat
Ask anything about your storage:
- *"What's taking up the most space?"*
- *"Do I have large video files in Downloads?"*
- *"Where are my iPhone backups?"*
- *"Is it safe to delete Xcode DerivedData?"*

---

## Privacy

- Runs entirely on your Mac — no account, no cloud sync
- Scan data stored locally in `~/Library/Application Support/MemoryOS/`
- AI responses use OpenAI — only category totals and folder sizes are sent, never file contents or full paths
