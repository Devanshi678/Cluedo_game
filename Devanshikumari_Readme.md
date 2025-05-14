# Cluedo Game - Project 2 (Part 1)

**Author:** Devanshikumari Patel  
**Language:** Python  
**Project Folder:** Devanshikumari_Project2_SourceCode

---

## 🎮 About the Game

This is a Python-based digital adaptation of the classic mystery-solving board game Cluedo (Clue). In this multiplayer game, players assume the role of characters who move across various rooms of a mansion, trying to solve a murder mystery by deducing the correct combination of suspect, weapon, and room.

---
## Game Objective
Your mission is to uncover the hidden mystery by:

-> Identifying who committed the murder

-> Determining which weapon was used

-> Pinpointing the location (room) where the murder took place

-> The correct combination is generated randomly at the start of the game and hidden from all players.
## 🗂️ Folder Structure

```
Devanshikumari_Project2_SourceCode/
├── game/
│   ├── main.py         # Game loop and player interaction
│   ├── board.py        #Room names and connections
│   ├── player.py       #Player class with movement and state
│   ├── characters.py   #Character definitions and start rooms 
│   ├── weapons.py      #List of possible weapons
│   ├── mystery.py      #Random generation of correct murder solution
│   └── suggestion.py   #Suggestion and refutation logic
├── Devanshikumari_Readme.md
```

---

## 🛠️ How to Run the Game

### ✅ Requirements

- Python 3 installed on your laptop
- No external libraries needed

### 💻 Steps

1. Open your terminal or command prompt  
2. Navigate to the project folder:

```bash
cd Devanshikumari_Project2_SourceCode
```

3. Run the game:

```bash
python game/main.py
```

4. Follow the prompts to choose a character, move between rooms, and make a suggestion.

---

## 📌 Game Instructions

- Your goal is to correctly guess the **murderer**, **weapon**, and **room**.
- The correct solution is chosen randomly each game.
- You can move between rooms and make one suggestion per turn.

## 📜 Game Rules Summary

- Each player is assigned a character and receives a set of clue cards.

- A random suspect, weapon, and room are selected as the true solution.

- On each turn, a player can:

        - Move to a connected room

        - Make a suggestion based on their current room

        - Make an accusation if they believe they know the solution

- Other players try to refute suggestions using their cards.

- If a player makes a correct accusation, they win.
- An incorrect accusation results in elimination.

##  Features Implemented
- Text-based interface with user prompts

- Modular code structure (logic divided into multiple files)

- Suggestion and refutation logic between players

- Correct and incorrect accusation handling

- Game ends on correct accusation or when all players are out

##  Testing Scenarios
- ✅ Valid suggestion and successful refutation

- ✅ Correct accusation that ends the game

- ⚠️ Edge case: Invalid character selection

- ⚠️ Edge case: Attempt to move to a non-connected room

- ⚠️ Edge case: Empty deck distribution logic

- ⚠️ Edge case: Handling zero players left in game
---