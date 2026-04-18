# Console Roulette Deluxe 🎰

A high-fidelity, interactive European Roulette game built entirely in C++ for the terminal. Experience the thrill of the casino with real-time arrow-key navigation, smooth animations, and integrated audio.

## ✨ Features

* **Interactive Table:** Use the **Arrow Keys** to move across the betting board. The current selection is highlighted in magenta.
* **Realistic Physics:** The wheel spin animation features a gradual slowdown effect to build suspense.
* **Audio Engine:** Powered by `miniaudio`, featuring background music, spinning sounds, and specific win/loss sound effects.
* **Smart UI:** Utilizing `SetConsoleCursorPosition` to prevent screen flickering and a clean "re-draw" system after every round.
* **Robust Logic:** * Full European Roulette rules (0-36).
    * Support for Straight-up bets, Columns, Even/Odd, and Red/Black.
    * Input validation to prevent crashes from accidental character entries.

## 🎮 Controls

| Key | Action |
| :--- | :--- |
| **↑ ↓ ← →** | Navigate the betting table |
| **Enter** | Select a spot and enter your bet amount |
| **X** | Cash out and exit the game |
| **R** | Restart game (only if you go bankrupt) |

## 🛠️ Installation & Setup

### Prerequisites
* A Windows environment (uses `<windows.h>` and `<conio.h>`).
* A C++ compiler (like MinGW/GCC).
* Audio files in the same folder as the executable:
    * `sound.wav` (Background music)
    * `spin.wav` (Spinning sound)
    * `jackpot.wav` (Win sound)
    * `fart.wav` (Loss sound)

### Building
Clone the repository and compile using the following command:

```bash
g++ main.cpp -o Roulette.exe -lwinmm