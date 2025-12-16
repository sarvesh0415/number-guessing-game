
# Number Guessing Game (Python)

This is a very simple number guessing game written in Python.  
This was my first GitHub repository, made while learning Python basics.

---

## What This Game Does

- The computer chooses a random number between 1 and 100
- You guess the number by typing it in the terminal
- The game tells you:
  - Lower number please → if your guess is too high
  - Higher number please → if your guess is too low
- When you guess correctly, the game ends and shows how many tries you took

---

## How to Run the Game

1. Download or clone the repository
2. Open the terminal in the project folder
3. Run the file
4. Start guessing numbers 🎯

---

## Note

This project was created while learning Python fundamentals like:

- Loops
- Conditions
- User input
- Random numbers

---

## Game Code

```python
import random

n = random.randint(1, 100)
a = -1
guesses = 0

while a != n:
    guesses += 1
    a = int(input("Guess a number: "))
    if a > n:
        print("Lower number please")
    else:
        print("Higher number please")

print(f"You have guessed the number in {guesses} attempts")
