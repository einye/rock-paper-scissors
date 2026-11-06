# Hand Gesture Rock-Paper-Scissors

A real-time Rock-Paper-Scissors game where you play using **hand gestures** in front of your webcam — no keyboard, no mouse, no controller. Built with [OpenCV](https://opencv.org/) and [MediaPipe](https://developers.google.com/mediapipe).

## How to Play

1. Run the script and position your hand(s) in view of the webcam.
2. A countdown will begin: **"Ready Players?" → Rock... → Paper... → Scissors... → SHOOT!"**
3. Show your gesture on **"SHOOT!"** (frame 60).
4. The winner is announced and the round restarts.

### Supported Gestures
| Gesture | Hand Shape |
|---------|------------|
| Rock | Fist (no fingers raised) |
| Scissors | Index + middle fingers raised (a peace sign is better detected :) |
| Paper | At least four fingers raised |

### Game Modes
- **1 Player** — Play against the computer (random move).
- **2 Player** — Both players show a hand at the same time; winner is decided locally.

The mode is chosen automatically based on how many hands are detected at the "SHOOT!" moment.

## Requirements

- Webcam
- **Python 3.12** (recommended — installs cleanly without dependency conflicts)

## Installation

```bash
# Clone the repo
git clone https://github.com/einye/rock_paper_scissors.git
cd rock_paper_scissors

# (Recommended) Create a virtual environment
python3.12 -m venv .venv
\.venv\Scripts\Activate.ps1        # Windows\VSCode\PowerShell_Terminal

# Install dependencies
pip install -r requirements.txt