# Memory Game Simulation

A JavaFX-based memory game simulation where players can play locally, compete against an AI, or simulate games between AI players. This project includes a graphical user interface, animations, and sound effects, providing an interactive and engaging experience.

## Features

- **Game Modes:**
  - Play vs. Computer: Choose AI difficulty (Easy, Medium, Hard, Impossible).
  - Play vs. Player: Two players share the same computer.
  - Simulation: Run AI vs. AI simulations to analyze win rates and export results to a CSV file.
  - Play Online: Placeholder for future implementation.
- **Customizable Simulations:** Configure the number of games and difficulty levels for AI players.
- **Graphical Interface:** Built with JavaFX, featuring animations and sound effects.
- **Settings Menu:** Adjust music, sound effects, and master volume.
- **Data Export:** Optionally export simulation results to a CSV file for further analysis.

## How the Game Works

1. There are 8 cards, numbered 1 through 8, placed face down.
2. Players take turns picking cards.
3. Players aim to collect the cards in ascending order (1, 2, 3, ..., 8).
4. After viewing a card, the player places it back in the same spot.
5. The game continues until one player successfully collects all cards in order.
6. Simulations analyze outcomes between different AI difficulties and turn order impacts.

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
   javac src/**/*.java
   java src.main.Main
   ```

## Usage

- Select a game mode from the main menu:
  - Play vs. Computer: Compete against an AI opponent with selectable difficulty.
  - Play vs. Player: Two players take turns on the same computer.
  - Simulation: Configure and run AI vs. AI games to analyze outcomes.
  - Settings: Adjust volume levels and sound preferences.
- For simulations, specify:
  - AI difficulty for both players.
  - Number of games to simulate.
  - Export results to a CSV file for further analysis.

## Example Output

```
Simulation Results:
Player 1 Wins: 53.4%
Player 2 Wins: 46.6%
Total Games Played: 10,000
```

## Future Improvements

- Add online multiplayer functionality.
- Allow for different deck sizes or custom rules.
- Enhance AI strategies for more realistic play styles.
- Add visual and sound customizations for a more immersive experience.

## License

This project is licensed under the MIT License

## Contributing

Contributions are welcome! If you'd like to contribute, please:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with a detailed description of your changes.

## Acknowledgments

This project was inspired by the curiosity of analyzing memory games and their outcomes under different conditions, and by the desire to create a visually appealing, interactive JavaFX application.
