# Number Guessing Game 🎲

A command-line Number Guessing Game built in **Bash** with a **PostgreSQL** database backend, developed as part of the Relational Database certification projects on **freeCodeCamp**.

---

## 🚀 Features
- **Interactive Gameplay**: Prompts users for a username, welcomes back returning players, and tracks their performance.
- **Dynamic Database Integration**: Stores user statistics securely using PostgreSQL, including total games played and the best game (fewest guesses).
- **Integer Validation**: Ensures robust user input handling.

---

## 🛠️ Technologies Used
- **Bash Scripting** (`number_guess.sh`)
- **PostgreSQL** (`psql` & `pg_dump` for database management)
- **Git** (Version control with structured conventional commits)

---

## 📋 Database Schema
The `number_guess` database contains a `users` table with the following columns:
- `user_id`: Primary key (Serial)
- `username`: Unique username (VARCHAR 22)
- `games_played`: Total number of games played (INT)
- `best_game`: Fewest number of guesses required to win (INT)

---

## 🎮 How to Run
1. Make sure PostgreSQL is running and you have the database set up:
   ```bash
   psql --username=freecodecamp --dbname=postgres -c "CREATE DATABASE number_guess;"

