# 🐍 Snake Game in Assembly (TASM/NASM)

## 🎮 Overview
This is a **classic Snake Game** written in **x86 Assembly Language** using **TASM/NASM**. The game runs in **real mode** and utilizes **video memory manipulation** to display the game on the screen.

## 🔥 Features
- **Classic Snake Movement** (Up, Down, Left, Right)
- **Food Generation & Eating Mechanism**
- **Score Display**
- **Game Over Condition** (Collision Detection with Walls & Itself)
- **Border Rendering**
- **Custom Messages & UI Elements**
- **Optimized Screen Clearing & Printing Functions**

## 🚀 How to Run
### 🛠 Prerequisites
Make sure you have the following installed:
- **TASM** (Turbo Assembler) or **NASM** (Netwide Assembler)
- **DOSBox** (For running in an emulated DOS environment)

### 💻 Steps to Run in DOSBox
1. **Download & Install DOSBox** if not already installed.
2. **Assemble the Code**:
   ```bash
   tasm snake_game.asm
   tlink snake_game.obj
   ```
   _(For NASM users, adjust accordingly)_
3. **Run the Game**:
   ```bash
   snake_game.exe
   ```
4. **Control the Snake** using **Arrow Keys**.
5. **Exit the Game** by pressing `ESC`.

## 📜 Controls
| Key | Action |
|-----|--------|
| ⬆️  | Move Up |
| ⬇️  | Move Down |
| ⬅️  | Move Left |
| ➡️  | Move Right |
| ESC | Exit Game |

## 🏆 Scoring System
- Score increases when the snake eats food.
- The **score is displayed** on the screen.

## 🛑 Game Over Conditions
- **Colliding with Walls** (Borders)
- **Hitting Own Body**

## ⚙️ Code Breakdown
### 🖥️ Graphics Handling
- Uses **video memory (0xB800)** for text-based graphics.
- **Custom `clrscr` function** to clear the screen.
- **`printstr` function** for rendering text at specific locations.

### 🏗️ Core Functions
| Function | Description |
|----------|-------------|
| `clrscr` | Clears the screen |
| `printstr` | Prints a string at a specific location |
| `print_score` | Displays the current score |
| `boarder_printing` | Draws game borders |
| `snake_move_*` | Handles snake movement (Up, Down, Left, Right) |
| `check_dead_element` | Detects game-over conditions |
| `random_function` | Generates random food positions |
| `display_food` | Displays food at a random location |

### 🎮 Game Flow
1. **Initialize Game & Print Borders**
2. **Show Instructions**
3. **Start the Snake & Food Rendering**
4. **Handle User Input for Movement**
5. **Detect Collisions & Update Score**
6. **Game Over if Collision Occurs**

## 🛠 Possible Enhancements
- ✅ **Increase Snake Speed Dynamically**
- ✅ **Add More Obstacles**
- ✅ **Multiplayer Mode**
- ✅ **Better Graphics Using VGA Mode**
- ✅ **Save High Scores**

## 🔥 Contributors
- **Designed by:** [Your Name]
- **Student Roll Numbers:** `21F-9132`, `21F-9214`

## 📜 License
This project is released under the **MIT License**. Feel free to modify and improve it!

## 🚀 Enjoy the Game! 🐍🎮

