# doom-python

A Doom-inspired 2.5D game engine built entirely in Python using ray-casting techniques, recreating the classic retro FPS experience of DOOM (1993).

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![Pygame](https://img.shields.io/badge/Pygame-2.0+-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## 📸 Screenshots

<p align="center">
  <img src="screenshots/1.png" width="45%" alt="Gameplay Screenshot 1">
  <img src="screenshots/2.png" width="45%" alt="Gameplay Screenshot 2">
</p>
<p align="center">
  <img src="screenshots/3.png" width="45%" alt="Gameplay Screenshot 3">
</p>

## 🎮 About the Project

This project simulates a pseudo-3D environment by projecting 2D map data into a first-person view using **ray casting**, the same core rendering technique used in legendary early FPS engines like Doom and Wolfenstein 3D.

Built as an educational exploration of classic game engine architecture, this project demonstrates:

- How early FPS engines rendered 3D worlds from 2D data
- Real-time rendering using mathematical ray-casting algorithms
- Player movement, rotation, and collision detection systems
- Game loops and event handling in Python

This is a learning project focused on understanding fundamental game engine concepts rather than replicating the full DOOM experience.

## 🛠 Tech Stack

- **Language:** Python 3.7+
- **Library:** Pygame
- **Rendering Technique:** Ray Casting (2.5D Engine)

## ✨ Features

- 🎯 First-person Doom-style movement and controls
- 🖱️ Mouse-based camera rotation for immersive gameplay
- 🧱 Ray-casted wall rendering with realistic depth perception
- 🎮 Smooth keyboard and mouse controls
- 🧠 Lightweight and educational game engine architecture
- 🕹 Authentic retro FPS visual style

## 🎮 Controls

| Input | Action |
|-------|--------|
| `W` | Move Forward |
| `S` | Move Backward |
| `A` | Move Left |
| `D` | Move Right |
| **Mouse** | **Rotate Camera / Look Around** |
| `ESC` | Quit Game |

## 📂 Project Structure

```
doom-python/
│
├── main.py              # Entry point and game loop
├── settings.py          # Game configuration and constants
├── raycasting.py        # Ray casting rendering logic
├── map.py               # Map layout and level data
├── player.py            # Player movement, rotation & physics
├── assets/              # Textures and game resources
├── README.md            # Project documentation
└── .gitignore           # Git ignore rules
```

## 🚀 Getting Started

### Prerequisites

- Python 3.7 or higher
- pip package manager

### Installation

**1. Clone the repository**

```bash
git clone git@github.com:RELXOP/doom-python.git
cd doom-python
```

**2. Create a virtual environment (recommended)**

```bash
python3 -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

**3. Install dependencies**

```bash
pip install pygame
```

**4. Run the game**

```bash
python main.py
```

## 🎯 How It Works

The engine uses **ray casting** to create the illusion of 3D:

1. The player's position and viewing angle are tracked in a 2D map
2. For each vertical column on the screen, a ray is cast from the player's position
3. The ray travels until it hits a wall in the 2D map
4. The distance to the wall determines the height of the wall slice drawn on screen
5. Closer walls appear taller, creating depth perception

This technique allows for fast rendering on limited hardware while creating an immersive 3D experience.

## 🔮 Future Improvements

- [ ] Textured walls and sprite rendering
- [ ] Enemy AI and pathfinding
- [ ] Weapons and shooting mechanics
- [ ] Sound effects and background music
- [ ] External map file loading system
- [ ] Performance optimizations
- [ ] Minimap display
- [ ] Lighting effects
- [ ] Mouse sensitivity settings

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/RELXOP/doom-python/issues).

## ⚠️ Disclaimer

This project is:
- **Fan-made and non-commercial**
- Created for educational purposes only
- Inspired by the original DOOM by id Software
- Does not use any original game assets

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Pragyan Kumar Biswas**

- GitHub: [@RELXOP](https://github.com/RELXOP)

## ⭐ Show Your Support

If you found this project interesting or helpful, please give it a ⭐ on GitHub! It helps others discover the project and motivates continued development.

---

*Built with curiosity and passion for classic game development* 🎮
