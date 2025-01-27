# Memory Game Simulation

A Java-based simulation to analyze the win rate of two perfect players in an 8-card memory game. This project explores how turn order impacts winning probabilities through computational modeling and statistical analysis.

## Features

- **Perfect Play Logic:** Simulates two players playing the memory game perfectly.
- **Turn-Based Simulation:** Alternates turns between the players, who aim to collect cards in ascending order (1 through 8).
- **Win Rate Analysis:** Runs multiple iterations of the game to compute and display win rates for the first and second player.
- **Customizable Settings:** Configure the number of cards, players, or simulation parameters.
- **Data Export:** Optionally export the results to a CSV file for further analysis.

## How the Game Works

1. There are 8 cards, numbered 1 through 8, placed face down.
2. Two players take turns picking cards.
3. Players aim to collect the cards in ascending order (1, 2, 3, ..., 8).
4. After viewing a card, the player places it back in the same spot.
5. The game continues until one player successfully collects all cards in order.
6. If both players play perfectly, this simulation analyzes who is more likely to win based on turn order.

## Project Structure

```
memory-game-simulation-java/
├── src/
│   ├── main/
│   │   └── Main.java              // Entry point of the JavaFX application
│   ├── controller/
│   │   ├── GameController.java    // Core simulation and game logic
│   │   ├── SimulationEngine.java  // Handles computer vs computer simulations
│   │   ├── OnlineGameController.java // Placeholder for future online gameplay logic
│   ├── model/
│   │   ├── Card.java              // Represents an individual card
│   │   ├── Deck.java              // Manages the collection of cards
│   │   ├── Player.java            // Abstract class for common player behavior
│   │   ├── HumanPlayer.java       // Represents a human player
│   │   ├── AIPlayer.java          // Implements AI behavior for various difficulties
│   ├── view/
│   │   ├── MainMenu.java          // JavaFX screen for game mode selection
│   │   ├── GameScreen.java        // JavaFX screen for the main game UI
│   │   ├── SimulationScreen.java  // JavaFX screen for simulation setup and execution
│   │   ├── SettingsScreen.java    // JavaFX screen for sound and volume settings
│   │   ├── ResultScreen.java      // JavaFX screen for simulation results and CSV export
│   ├── utils/
│   │   ├── SoundManager.java      // Manages background music and sound effects
│   │   ├── AnimationManager.java  // Handles animations for cards and transitions
│   │   ├── CSVExporter.java       // Exports simulation data to a CSV file
│   │   └── MediaLoader.java       // Loads and manages images and sound resources
├── README.md                      // Project overview and instructions
├── LICENSE                        // License for the repository
└── .gitignore                     // Files to exclude from version control
```

## Getting Started

### Prerequisites

To run this project, you'll need:
- Java Development Kit (JDK) 11 or later
- An IDE such as IntelliJ IDEA, Eclipse, or VS Code (optional but recommended)

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/memory-game-simulation-java.git
   ```

2. Navigate to the project directory:
   ```bash
   cd memory-game-simulation-java
   ```

3. Open the project in your favorite IDE.

4. Compile and run the project:
   ```bash
   javac src/*.java
   java src.Main
   ```

## Usage

- Modify the simulation parameters (e.g., number of games, number of cards) in `GameSimulation.java`.
- Run the program to simulate the game and analyze the win rates.
- View the results in the console or export them for further analysis.

## Example Output

```
Simulation Results:
Player 1 Wins: 53.4%
Player 2 Wins: 46.6%
Total Games Played: 10,000
```

## Future Improvements

- Add a graphical user interface (GUI) using JavaFX.
- Allow for different deck sizes or custom rules.
- Compare results for players with imperfect memory.
- Add more statistical analysis and visualization options.

## License

This project is licensed under the MIT License

## Contributing

Contributions are welcome! If you'd like to contribute, please:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with a detailed description of your changes.

## Acknowledgments

This project was inspired by the curiosity of analyzing memory games and their outcomes under perfect conditions.
