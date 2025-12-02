# So Long

A small 2D game built with MinilibX where you guide a character to collect all items and reach the exit.

## 🎮 Getting Started

### Prerequisites

This project requires **MinilibX**, **X11**, and **Xext** libraries.
Make sure you have a C compiler (like `cc` or `gcc`) and `make` installed.

### Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd so_long
   ```

2. Compile the game:
   - For the standard version:
     ```bash
     make
     ```
   - For the bonus version (with animations and move counter):
     ```bash
     make bonus
     ```

## 🕹️ How to Play

Run the game by passing a map file as an argument:

```bash
./so_long maps/small.ber
```

Or for the bonus version:

```bash
./so_long_bonus maps/small.ber
```

### Controls

| Key | Action |
| --- | --- |
| **W** | Move Up |
| **A** | Move Left |
| **S** | Move Down |
| **D** | Move Right |
| **ESC** | Quit Game |
| **X (Window)** | Quit Game |

### Objective

- The goal is to collect all **collectibles (C)** on the map.
- Once all collectibles are gathered, the **exit (E)** opens.
- Reach the exit to win the game.
- Avoid obstacles (walls).

## 🗺️ Maps

The game uses `.ber` files to define the map layout.
- **1**: Wall
- **0**: Empty space
- **C**: Collectible
- **E**: Exit
- **P**: Player start position

Maps must be rectangular and surrounded by walls. Examples can be found in the `maps/` directory.

## ✨ Features

- **2D Graphics**: Simple tile-based rendering using MinilibX.
- **Movement**: Smooth player movement with collision detection.
- **Map Validation**: Checks if the map is valid (rectangular, enclosed, contains valid path).
- **Bonus Features**:
    - Sprite animations for the player.
    - Move counter display on the screen.

## 👨‍💻 Author

- **vmanuyko**
