# 🧠 Scrabble Score Tracker

This Python script implements a simple Scrabble-style scoring system. It assigns point values to letters, calculates word scores, and tracks the performance of multiple players.

---

## 📌 Features

- ✅ Calculates the score of individual words based on Scrabble letter values
- ✅ Tracks words played by each player
- ✅ Computes total points for each player
- ✅ Allows new words to be added and updates scores dynamically

---

## 🧮 How It Works

1. **Letter Scoring**  
   Each letter is assigned a point value (e.g. A=1, B=3, C=3, etc.). Both uppercase and lowercase letters are supported.

2. **Score Calculation**  
   The `score_word()` function returns the total score for a given word.

3. **Tracking Player Words**  
   A dictionary called `player_to_words` keeps track of each player and the words they’ve played.

4. **Score Updating**  
   The `update_point_totals()` function calculates total points for each player and updates `player_to_points`.

5. **Adding New Words**  
   The `play_word()` function adds a new word for a player and updates their score.

---

## ▶️ Example Usage

```python
score_word("BROWNIE")           # Returns 15

player_to_words["player1"]      # ['BLUE', 'TENNIS', 'EXIT']

update_point_totals()           # Recalculate all player scores

play_word("player1", "PYTHON")  # Adds "PYTHON" to player1's words and updates scores
