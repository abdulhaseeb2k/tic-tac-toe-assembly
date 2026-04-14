# Tic Tac Toe in Assembly

## Project Documentation

### Features
- Single-player mode against AI
- Two-player mode
- Displays the game board in the console
- Determines winner and provides game result

### Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/abdulhaseeb2k/tic-tac-toe-assembly.git
   cd tic-tac-toe-assembly
   ```
2. Install necessary tools:
   - Ensure you have an assembler (like NASM) installed.

3. Assemble the project:
   ```bash
   nasm -f elf64 -o tic_tac_toe.o tic_tac_toe.asm
   ```

4. Link the object file:
   ```bash
   ld -o tic_tac_toe tic_tac_toe.o
   ```

5. Run the game:
   ```bash
   ./tic_tac_toe
   ```

### How to Play
- The game is played on a 3x3 grid.
- Players take turns placing their mark (X or O) in an empty square.
- The first player to align three marks horizontally, vertically, or diagonally wins the game.
- If the grid is full and no player has aligned three marks, the game is a draw.

### Code Overview
This project is implemented in Assembly Language. The main components of the code include:
- **Display functions** to render the game board in the console.
- **Input handling** for player moves.
- **Game logic** to check for wins and draws.

### Contributing Guidelines
Contributions are welcome! Please follow these guidelines:
1. Fork the repository
2. Create a new feature branch (`git checkout -b feature-YourFeature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature-YourFeature`)
6. Open a Pull Request

### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.