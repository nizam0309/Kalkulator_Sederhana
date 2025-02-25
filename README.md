# Kalkulator_Sederhana
Kalkulator Web
This is a simple calculator application built using HTML, CSS, and JavaScript. The calculator allows basic arithmetic operations like addition, subtraction, multiplication, and division. It includes a sleek design and supports standard operations and error handling.

Features
Addition, subtraction, multiplication, and division.
Clear all input with the "AC" button.
Backspace functionality to remove the last digit entered.
Real-time result calculation using the "=" button.
Error handling when an invalid expression is entered.
Clean and responsive design.
File Structure
index.html: The main HTML file containing the structure and layout of the calculator.
style: Internal CSS styling used to format the calculator’s appearance.
script: Internal JavaScript used to handle the logic for the calculator.
How It Works
HTML:

The layout consists of a main div container (calculator) that holds the input display and buttons.
Buttons for digits (0-9), operators (+, -, *, /), and other functionality like clear (AC) and backspace (C).
The equal (=) button is used to calculate the result.
CSS:

The styling is centered around a clean and modern design. The calculator has a red background with rounded corners, shadow effects, and white buttons.
Flexbox and Grid are used to ensure a responsive layout, aligning the elements efficiently on different screen sizes.
JavaScript:

appendToDisplay(value): Appends the clicked button value to the display.
ClearDisplay(): Clears the input display.
backspace(): Removes the last character from the input display.
calculateResult(): Uses eval() to calculate the expression and display the result. If the expression is invalid, an error message is shown.
How to Use
Open the index.html file in any modern web browser (e.g., Chrome, Firefox, etc.).
Use the number buttons (0-9) and operators (+, -, *, /) to input an expression.
Press the "=" button to calculate the result.
Press "AC" to clear the display.
Press "C" to delete the last entered character.
The result will be displayed in the input box.
Example
Simple Calculation:
Input: 3 + 5
Press "="
Output: 8
Invalid Input:
Input: 3 +
Press "="
Output: Error Boss
Notes
The eval() function is used to evaluate the expression. It is generally safe for basic arithmetic but should be used carefully in production environments to avoid security risks.
The calculator does not support complex expressions like parentheses or advanced mathematical functions. It's a simple, straightforward calculator.
License
This project is open source and available under the MIT License.
