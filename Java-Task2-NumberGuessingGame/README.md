# Number Guessing Game (Java)

A console-based number guessing game built in Java for the **Oasis Infobyte Student Internship Program (OIBSIP)**, Task 2.

The computer picks a secret number, and you try to guess it within a limited number of attempts. Pick a difficulty, play as many rounds as you like, and track your results on a scoreboard.

## Features

- Random secret number generated at the start of every round
- **Too High! / Too Low! / Correct!** hints after each guess
- Attempt counter shown on every prompt (e.g. `Attempt 3/7`)
- Maximum attempts limit; the secret number is revealed if you lose
- **Three difficulty levels** (Easy, Medium, Hard)
- **Play Again** option after every round
- **Scoreboard** that tracks every round (won or lost, attempts used, difficulty) and your total wins
- Input validation: non-numeric or out-of-range input is rejected without crashing the game
- Graceful exit if input is closed (Ctrl+D / Ctrl+Z)

## Difficulty Levels

| Level  | Number Range | Max Attempts |
|--------|--------------|--------------|
| Easy   | 1 - 50       | 10           |
| Medium | 1 - 100      | 7            |
| Hard   | 1 - 200      | 5            |

## Requirements

- Java JDK 8 or higher

## How to Run

```bash
javac NumberGuessingGame.java
java NumberGuessingGame
```

## How to Play

1. Choose a difficulty (1, 2, or 3).
2. Enter your guess when prompted.
3. Use the **Too High! / Too Low!** hints to narrow it down before you run out of attempts.
4. After the round, view the scoreboard and choose whether to play again (`yes` / `no`).
5. When you quit, the final scoreboard is displayed.

## Sample Output

```
=====================================
      WELCOME TO NUMBER GUESSING
=====================================

Choose difficulty:
  1) Easy   (1-50, 10 attempts)
  2) Medium (1-100, 7 attempts)
  3) Hard   (1-200, 5 attempts)
Enter choice (1-3): 2

--- Round 1 (Medium) ---
I'm thinking of a number between 1 and 100. You have 7 attempts.
Attempt 1/7 - Your guess: 50
Too Low!
Attempts left: 6
Attempt 2/7 - Your guess: 75
Too High!
Attempts left: 5
Attempt 3/7 - Your guess: 63
Correct! You got it in 3 attempts.

========== SCOREBOARD ==========
Round 1 - guessed in 3 attempts [Medium]
--------------------------------
Won 1 of 1 round
================================

Play again? (yes/no):


