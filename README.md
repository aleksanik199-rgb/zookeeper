# Zookeeper 🦁

A console application in Kotlin that simulates zoo habitat cameras: the user enters a habitat number and sees an ASCII-art "camera feed" of the animal living there. Built as a learning project on the Hyperskill (JetBrains Academy) platform.

## What it does

1. The program asks the user to enter the number of the habitat they want to view.
2. It prints an ASCII-art scene of the corresponding animal (camel, lion, deer, goose, bat or rabbit).
3. The loop repeats, so the user can check as many habitats as they like.
4. Typing `exit` stops the program.

## Project structure

- `Zookeeper.kt` — the whole program. Six `const val` string constants hold the ASCII art (one per animal), collected into the `animals` array. The `main` function runs a `while (true)` loop that reads input, checks for `exit`, and otherwise prints `animals[input.toInt()]`.

## How to run

1. Install IntelliJ IDEA (or another Kotlin-capable IDE).
2. Clone the repository or copy `Zookeeper.kt` into a Kotlin project.
3. Run the `main` function.
4. Enter a habitat number (0–5) to see the animal, or type `exit` to quit.

## Known limitations

- No input validation: entering a non-numeric value crashes the program with `NumberFormatException`, and a number outside 0–5 crashes it with `ArrayIndexOutOfBoundsException`.

## What I practiced

Multiline strings with triple quotes, arrays, an infinite loop with `break`, and indexing into a collection by user input.