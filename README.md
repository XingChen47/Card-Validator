# Card-Validator

A C++ program to validate card numbers for correct format and validity. This utility checks if a card number is valid using the Luhn algorithm.

## Features

- Validates card numbers using the Luhn algorithm
- Simple command-line interface for user interaction
- Cross-platform: works on Linux, Windows, and macOS

## Installation

### 1. Clone the repository
```sh
git clone https://github.com/XingChen47/Card-Validator.git
cd Card-Validator
```

### 2. Compile the program

#### **Linux/macOS**
```sh
g++ -o Card_Validator "Credit Card Validator.cpp"
```

#### **Windows (using MinGW)**
```sh
g++ -o Card_Validator.exe "Credit Card Validator.cpp"
```
*Make sure `g++` is available in your PATH. If using another compiler, adjust the command accordingly.*

## Usage

You can run the program in two ways:

### **Interactive Mode:**  
Simply run the compiled program and follow the prompt to enter a card number.

**Linux/macOS:**
```sh
./Card_Validator
```

**Windows:**
```sh
Card_Validator.exe
```

### **Command-Line Argument:**  
Pass the card number as a command-line argument.

**Linux/macOS:**
```sh
./Card_Validator 4111111111111111
```

**Windows:**
```sh
Card_Validator.exe 4111111111111111
```

## How it Works

1. **Format Validation:** Checks the length and ensures all characters are numeric.
2. **Luhn Algorithm:** Applies the Luhn algorithm to verify the validity of the card number.
