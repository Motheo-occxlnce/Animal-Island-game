# Animal-Island-game

A browser-based logic puzzle game inspired by the classic **Magnavox Odyssey "Animal Island"** river-crossing challenge. Move all seven animals across a chain of islands from the starting pen to the final cage — without letting any predator eat its prey along the way.

## About the Project

This is a single-file HTML/CSS/JavaScript implementation of the Animal Island puzzle. It runs entirely in the browser with no dependencies, no build step, and no server required. Just open the file and play.

The project's purpose is to faithfully recreate the original Odyssey instruction-screen rules in a modern web format, while extending the classic 6-animal version to a 7-animal variant that includes a donkey.

## How to Play

Open `animal_island_odyssey_game.html` in any modern web browser. That's it.

The goal is to transport all seven animals — Lion, Bird, Elephant, Jackal, Dog, Cat, and Donkey — from the starting pen (left) to the final cage (right) by routing them through three middle islands.

### Controls

Click an animal to select it (it will highlight in blue and appear in the boat). Then click an island to move the selected animal there. Use the **RESET** button to start over and **UNDO** to take back your last move. The **INSTRUCTIONS** button displays the rules in-game.

### Rules

1. Move only one animal at a time.
2. Forward moves go exactly one island at a time.
3. Backward moves can jump to any previous island.
4. On the numbered middle islands, an animal can only move forward if there is a companion already on that island — *unless* it is the last animal in the chain (no animals behind it), in which case it may advance alone.
5. Animals attack each other only on the three middle islands. The starting pen and final cage are safe zones.

### Predator Rules

- **Lion** eats Jackal, Dog, Cat, and Donkey (but not Bird or Elephant)
- **Jackal** eats Dog and Cat
- **Dog** eats Cat and Bird
- **Cat** eats Bird
- **Bird, Elephant, Donkey** are non-predatory

If a predator and its prey are ever left together on a middle island, the game ends.

## Project Structure

```
.
├── animal_island_odyssey_game.html   # The complete game (HTML + CSS + JS in one file)
└── README.md                          # This file
```

## Tech Stack

Plain HTML, CSS, and vanilla JavaScript. No frameworks, no libraries, no build tools.

## License

This is a fan recreation of a puzzle from the 1972 Magnavox Odyssey console. The code is provided as-is for educational and personal use.

