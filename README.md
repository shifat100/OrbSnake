# OrbSnake

A minimalist, dot-matrix Snake game built in a **single HTML file** with zero external dependencies. Inspired by clean modern dot-grid interfaces, **OrbSnake** blends flat 2D vector aesthetics with a smooth real-time **3D sphere mode**, seamless **wrap-around edges**, and full **T9 feature-phone keypad**, keyboard, and touch support.

---

## Features

- **Dot-Matrix Wave Loading Screen**
  - Continuous diagonal wave animation across an adaptive dot grid (`0%`–`100%`).
  - Always preserves subtle base dots across the entire viewport, even on ultra-small screens (`128×160`, `240×320`).
- **Seamless 2D ↔ 3D Mode Toggle**
  - Switch smoothly mid-game without losing progress or resetting your score.
  - **2D Mode:** Flat royal-blue circular segments on a crisp white dot grid.
  - **3D Mode:** Tilted perspective board, glossy 3D shaded spheres, projected floor shadows, depth sorting, and a floating food orb.
- **Wrap-Around Borders**
  - Moving past any edge wraps smoothly onto the opposite side with clipped sub-grid animation.
  - Game over occurs only upon self-collision (turning the snake translucent grey with `× ×` eyes).
- **Full T9 Keypad, Keyboard & Touch Controls**
  - Built to work effortlessly on KaiOS / feature phones, PC numpads, standard keyboards, and mobile touchscreens.
- **Persistent High Score**
  - Automatically saves your `Best` score locally using `localStorage`.
- **Zero Dependencies**
  - 100% pure HTML5 `<canvas>`, CSS3, and Vanilla JavaScript in one lightweight file.

---

## Controls

| Action | T9 Keypad | Keyboard | Touch / Mouse |
| :--- | :---: | :---: | :---: |
| **Move Up** | `2` | `↑` / `W` | Swipe Up |
| **Move Down** | `8` | `↓` / `S` | Swipe Down |
| **Move Left** | `4` | `←` / `A` | Swipe Left |
| **Move Right** | `6` | `→` / `D` | Swipe Right |
| **Pause / Resume** | `5` / `*` / `SoftLeft` | `Enter` / `Space` | — |
| **Play Again (Game Over)** | `5` / `SoftLeft` | `Enter` / `Space` | Tap **Play Again** |
| **Toggle 2D ↔ 3D Mode** | `0` | `0` | **Press & Hold for 5s** |
| **Instant Restart** | `#` / `SoftRight` | `#` | — |
| **Skip Loading Screen** | `5` / `*` / `SoftLeft` | `Enter` | — |

> **Tip:** When holding on the touchscreen or mouse to switch between **2D** and **3D** mode, keep your finger still—a subtle blue circular ring will appear after `0.45s` to track the 5-second countdown. Swiping cancels the hold immediately so gameplay is never interrupted.

---

## How to Run

1. Save the game code as `index.html`.
2. Open `index.html` in any modern web browser (Desktop, Mobile, or Feature Phone browser).

Or run a quick local server if needed:

```bash
# Using Python 3
python3 -m http.server 8080
```

Then visit `http://localhost:8080` in your browser.

---

## Responsive Design

OrbSnake automatically scales its dot-matrix grid and UI pills to fit:
- **Ultra-small feature phone screens** (`128×160`, `240×320`)
- **Modern smartphones** (portrait & landscape)
- **Tablets and desktop monitors** (with HiDPI / Retina `devicePixelRatio` support)

---

## License

This project is open-source and available under the [MIT License](LICENSE).
