# card-validator

A C++ program to validate card numbers for correct format and validity. This utility checks if a card number is valid using the Luhn algorithm and can identify card types (such as Visa and MasterCard) based on their number prefixes.

## Features

- Validates card numbers using the Luhn algorithm
- Detects card type (Visa, MasterCard, etc.) based on number prefix
- Simple command-line interface for user interaction
- Cross-platform: works on Linux, Windows, and macOS

## Installation

### 1. Clone the repository
```sh
git clone https://github.com/XingChen47/card-validator.git
cd card-validator
```

### 2. Compile the program

#### **Linux/macOS**
```sh
g++ -o card_validator "Credit Card Validator.cpp"
```

#### **Windows (using MinGW)**
```sh
g++ -o card_validator.exe "Credit Card Validator.cpp"
```
*Make sure `g++` is available in your PATH. If using another compiler, adjust the command accordingly.*

## Usage

You can run the program in two ways:

### **Interactive Mode:**  
Simply run the compiled program and follow the prompt to enter a card number.

**Linux/macOS:**
```sh
./card_validator
```

**Windows:**
```sh
card_validator.exe
```

### **Command-Line Argument:**  
Pass the card number as a command-line argument.

**Linux/macOS:**
```sh
./card_validator 4111111111111111
```

**Windows:**
```sh
card_validator.exe 4111111111111111
```

**Example Output:**
```
Card number: 4111111111111111
Card type: Visa
Valid: Yes
```

## How it Works

1. **Format Validation:** Checks the length and ensures all characters are numeric.
2. **Luhn Algorithm:** Applies the Luhn algorithm to verify the validity of the card number.

## Example

```sh
./card_validator 5500000000000004
```
Output:
```
Card number: 5500000000000004
Card type: MasterCard
Valid: Yes
```

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss your ideas.

## License

This project is licensed under the MIT License.
