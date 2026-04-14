# How to Run the Tic Tac Toe Assembly Program

This document provides comprehensive step-by-step instructions on how to run the Tic Tac Toe Assembly program on Linux, macOS, and Windows systems. Please follow the prerequisites and steps carefully.

## Prerequisites

### For Linux:
1. **Install NASM**:  Use the following command to install NASM (Netwide Assembler):  
   ```bash
   sudo apt-get install nasm
   ```
2. **Install GCC**: Use the package manager to install GCC if you haven't already:
   ```bash
   sudo apt-get install gcc
   ```

### For macOS:
1. **Install Homebrew**: If you don’t have Homebrew, you can install it using:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
2. **Install NASM and GCC**:
   ```bash
   brew install nasm gcc
   ```

### For Windows:
1. **Download NASM**: Download the NASM installer from [the NASM official website](https://www.nasm.us/).
2. **Install GCC**: Install MinGW or a similar package. Make sure to include the `bin` directory in your system's PATH variable during installation.

## Step-by-Step Instructions

### Step 1: Clone the Repository
Open your terminal or command prompt and run:
```bash
git clone https://github.com/abdulhaseeb2k/tic-tac-toe-assembly.git
cd tic-tac-toe-assembly
```

### Step 2: Assemble the Program
Run the following command to assemble the main.asm file:
```bash
nasm -f elf64 main.asm -o main.o  # For Linux and macOS
nasm -f win32 main.asm -o main.obj  # For Windows
```

### Step 3: Link the Program
Next, link the object file using GCC:
```bash
gcc main.o -o tictactoe  # For Linux and macOS
gcc main.obj -o tictactoe  # For Windows
```

### Step 4: Run the Program
Finally, run the executable:
```bash
./tictactoe  # For Linux and macOS
.
\tictactoe.exe  # For Windows
```

## Troubleshooting
- If you encounter errors during the assembly step, ensure that you are in the correct directory and that the assembly file is named properly.
- Check if NASM and GCC are correctly installed by running `nasm -v` and `gcc -v` in your terminal or command prompt.
- Make sure your PATH environment variable includes the directories where NASM and GCC are installed, especially on Windows.

## Conclusion
Follow these steps to successfully run the Tic Tac Toe assembly program on your respective operating system. If you encounter any issues, please refer to the troubleshooting section or seek help from community forums.