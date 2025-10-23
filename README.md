# Safe-Key-Capture
Safe Key Capture — a consent-first demo that logs keyboard events only while its Tkinter window is focused. It shows captured entries on-screen and saves timestamped key names and printable characters to `typed_log.txt`. Use only in documented, consented demos (user studies, tests, classes).


# Safe Key Capture — Consent-First Demo

> **Important:** This repository documents a consent-based, visible demo tool intended for educational use only.  
> Do **NOT** use this software to capture other people's input without explicit, informed consent. Misuse may be illegal and unethical.

## Project summary

**Safe Key Capture** is an educational demo showing how a GUI application can capture keyboard **events** while the app window is focused and display them in a visible log. The goal is to teach event handling, timestamping, and responsible data handling — not to enable covert monitoring.

This README explains the project purpose, safe usage rules, installation, and how to run a consented demonstration.


## Key principles / ethics

- **Consent first.** Only use this program with the clear, informed consent of everyone whose input may be recorded. Prefer written consent when appropriate.
- **Transparency.** The application shows an on-screen log of captured input so participants can see exactly what is recorded.
- **Scope-limited.** The demo records events only while the demo window is focused and the user is actively interacting with it.
- **Minimal retention.** Logs are stored locally in `typed_log.txt`. Delete logs after the demo unless participants agree otherwise.
- **No stealth features.** This demo must not be modified to run stealthily or as a background/global logger.

---

## What this repo contains

- `safe_key_capture.py` — an educational GUI app that demonstrates keyboard event handling and visible logging.  
  *Provided here for reference; do not use this outside of explicit, consented demos.*
- `typed_log.txt` — (created at runtime) local text file storing timestamped entries of captured events.
- `README.md` — this file.

---

## Intended audience

- Students learning event-driven programming (GUI and keyboard events).  
- Instructors demonstrating responsible data capture and privacy best practices.  
- Developers who want to learn how to log user input for explicit, consented testing scenarios (for example, user studies or accessibility testing).

---

## Installation

1. Ensure you have Python 3.8+ installed.
2. (Optional) Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate   # macOS / Linux
   .venv\Scripts\activate      # Windows (PowerShell)


## Safe usage / demo procedure (must be followed)

-Read and understand this README.
-Obtain explicit informed consent from every participant before any data capture begins. Explain what will be recorded, why, how the data will be stored, and when it will be deleted.
-Run the demo in view of the participant (no hidden screens).
-Use only the demo window while capturing — do not switch to other windows.
-After the demo, show the captured typed_log.txt to the participant and permanently delete the file if requested.


## What gets stored

Captured entries are written to typed_log.txt in the project folder. Each line should include:

-A human-friendly timestamp (local time).
-A readable key name (e.g., a, Return, Shift_L).
-A representation of the character (if printable).
-Before sharing logs, remove or redact any personally identifying or sensitive content.
