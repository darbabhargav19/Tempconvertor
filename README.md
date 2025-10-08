# Temperature Converter

A simple Python script to convert temperatures between Celsius and Fahrenheit based on user input.

## Description

This Python program allows users to input a temperature value and its unit (Celsius or Fahrenheit) and converts it to the other unit. The program handles invalid inputs by displaying an error message if an unrecognized unit is provided.

## Features

- Converts temperatures from Celsius to Fahrenheit and vice versa.
- Rounds the converted temperature to one decimal place for readability.
- Validates user input and displays an error for invalid units.

## Installation

1. Clone the repository:
   git clone https://github.com/darbabhargav19/Tempconvertor.git
2. Navigate to the project directory:
   cd <your-repo-name>
3. Ensure you have Python installed (version 3.x recommended). Check your Python version:
   python --version
   or
   python3 --version

## Usage

1. Run the script using Python:
   python temp_converter.py
   or
   python3 temp_converter.py
2. Follow the prompts:
   - Enter the unit of the temperature (C for Celsius or F for Fahrenheit).
   - Enter the temperature value.
3. The program will display the converted temperature or an error message if the unit is invalid.

### Example
Is this temperature in Celsius or Fahrenheit (C/F): C
Enter the temperature: 25
The temperature in Fahrenheit is: 77.0°F

Is this temperature in Celsius or Fahrenheit (C/F): F
Enter the temperature: 77
The temperature in Celsius is: 25.0°C

Is this temperature in Celsius or Fahrenheit (C/F): K
K is an invalid measurement

## Code

unit = input("Is this temperature in Celsius or Fahrenheit (C/F): ")
temp = float(input("Enter the temperature: "))

if unit == "C":
    temp = round((9 * temp) / 5 + 32, 1)
    print(f"The temperature in Fahrenheit is: {temp}°F")
elif unit == "F":
    temp = round((temp - 32) * 5 / 9, 1)
    print(f"The temperature in Celsius is: {temp}°C")
else:
    print(f"{unit} is an invalid measurement")

## Requirements

- Python 3.x
- No external libraries required

## Contributing

Contributions are welcome! If you'd like to improve this project, please follow these steps:
1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Make your changes and commit (git commit -m 'Add some feature').
4. Push to the branch (git push origin feature-branch).
5. Open a pull request.


## Acknowledgments

- Inspired by simple command-line utility projects.
- Thanks to the Python community for excellent resources and documentation.
