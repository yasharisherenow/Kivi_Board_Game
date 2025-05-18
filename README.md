# Kivi_Board_Game
---

# KIVI – Strategic Multiplayer Board Game (Java Executable)

**KIVI** is a Java-based digital adaptation of the award-winning board game, developed with an emphasis on strategic depth, user accessibility, and clean architectural design. This `.jar`-only release supports 2–4 players (human or AI), save/load functionality, and a scalable modular system that incorporates **software design patterns**, test-driven development, and accessible UI logic.

This project was built from scratch over multiple Agile sprints and is presented as a polished, standalone `.jar` file — no installation or setup required.

---

## Key Features

* **Multiplayer Engine (2–4 Players)**
  Built to support any mix of human-vs-human or human-vs-computer configurations. The game loop is dynamically managed using a clean controller-view separation and internal turn manager logic.

* **AI Opponent (Easy & Hard Difficulty)**

  * *Easy AI*: Selects valid moves randomly.
  * *Hard AI*: A deterministic Java-based decision engine that evaluates board states, detects threats, and simulates scoring potential.

* **Save & Resume Game**
  Players can persist their game state to disk at any time and resume without loss of progress. Aesthetic design touches and subtle feedback cues improve the user experience during load sequences.

* **Accessibility for Color Vision Deficiency**
  All color-dependent visuals are reinforced with shapes/symbols to ensure clarity for players with color blindness or low contrast sensitivity.

* **Unit Testing Coverage**
  Critical game systems — including AI logic, board validation, save/load mechanics, and player state transitions — were rigorously tested using **JUnit** to ensure stability and correctness.

* **Design Patterns Used**
  The system architecture incorporates several fundamental design patterns:

  * **Strategy Pattern** – for modular AI difficulty switching
  * **Singleton Pattern** – for centralized game state management
  * **Observer Pattern** – to update UI components in response to game events
  * **Factory Pattern** – for creating player instances based on user input
    These patterns improve extensibility, separation of concerns, and future scalability (e.g., networked multiplayer).

---

## How to Run

**Requirements:** Java 17+

1. Download the file: `KiviGame.jar`

2. Open your terminal or command prompt in the directory containing the `.jar`.

3. Run with:

   ```bash
   java -jar KiviGame.jar
   ```

---

## Gameplay Flow

1. **Start Screen**
   Configure the number of players, assign names, and choose AI difficulty where applicable.

2. **Turn-Based Play**
   Players alternate placing stones on the board, aiming to maximize scoring opportunities. The UI highlights valid moves and indicates turn transitions clearly.

3. **Save & Load**
   Use the in-game menu to save progress. You can load games from the main menu during a future session.

4. **Endgame & Scoring**
   When no valid moves remain, scores are automatically tallied and a winner is declared.

---

## Development Approach

* **Language**: Java
* **Testing**: JUnit
* **Methodology**: Agile (weekly sprint planning, iterative delivery, peer-reviewed pull requests)
* **Architecture**: OOP with layered design, modular responsibilities, and design pattern integration
* **UX Principles**: Focus on intuitive visuals, low cognitive load, and inclusivity

---

## About the Project

This project was developed as a final team capstone by **Group 13**. It reflects a professional standard of software quality, clean modularity, and thoughtful design. Though only the `.jar` is distributed, the underlying system demonstrates proficiency in AI logic, pattern-based software architecture, and full-stack game development — all in Java.

---

Let me know if you’d like a 1-paragraph “portfolio blurb” version for a resume, or a snappy one-liner for LinkedIn.
