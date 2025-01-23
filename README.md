# Simon Game

This is a simple implementation of the classic **Simon Game**, where players need to remember and repeat a sequence of colors. The game gets progressively more challenging as the sequence grows longer.

## Table of Contents
- [How to Play](#how-to-play)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Folder Structure](#folder-structure)
- [Setup](#setup)
- [Game Logic](#game-logic)
- [Future Enhancements](#future-enhancements)

---

## How to Play
1. Press any key to start the game.
2. Watch the sequence of colors flash on the screen.
3. Click the buttons in the correct order to repeat the sequence.
4. If you match the sequence, you move to the next level, and the sequence grows longer.
5. If you click the wrong button, the game will display "Game Over" and reset.

---

## Features
- **Dynamic Difficulty**: The game gets harder as the sequence grows with each level.
- **Sound Feedback**: Each button has an associated sound to help players remember the sequence.
- **Visual Effects**: Buttons flash when clicked or during the sequence playback.
- **Restart Functionality**: The game restarts automatically after a wrong answer.

---

## Technologies Used
- **HTML**: For structuring the webpage.
- **CSS**: For styling the buttons and the game interface.
- **JavaScript**: For implementing game logic.
- **jQuery**: For DOM manipulation and event handling.

---

## Folder Structure
```
project/
├── index.html       # Main HTML file
├── styles.css       # CSS styles
├── game.js          # Main JavaScript file
└── sounds/          # Audio files for button sounds
    ├── red.mp3
    ├── blue.mp3
    ├── green.mp3
    ├── yellow.mp3
    └── wrong.mp3
```

---

## Setup
1. Clone the repository or download the project files.
2. Ensure you have the following folder structure:
   - An `index.html` file for the webpage.
   - A `game.js` file for the JavaScript code.
   - A `sounds/` folder with the following audio files:
     - `red.mp3`
     - `blue.mp3`
     - `green.mp3`
     - `yellow.mp3`
     - `wrong.mp3`
3. Open `index.html` in a browser to start playing the game.

---

## Game Logic
### Main Components:
- **`nextSequence()`**: Generates a new color in the sequence, updates the game level, and plays the corresponding sound.
- **`checkAnswer(currentLevel)`**: Validates the user's input against the game sequence.
- **`playSound(colorName)`**: Plays the sound associated with the given color.
- **`animatePress(currentColor)`**: Adds a pressed effect to the clicked button.
- **`startOver()`**: Resets the game state after a wrong answer.

### Event Handlers:
- `keydown`: Starts the game when a key is pressed.
- `click`: Handles user input and triggers game logic.

---

## Future Enhancements
- Add a high-score tracker to display the best performance.
- Implement different difficulty modes (e.g., Easy, Medium, Hard).
- Add a timer to make the game more challenging.
- Enhance the UI/UX with animations and responsive design.

---

Enjoy playing the Simon Game! 🚀

