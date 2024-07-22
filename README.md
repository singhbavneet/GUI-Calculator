# GUI-Calculator
![cal py ss](https://github.com/user-attachments/assets/fa8adc8e-47ff-47a1-8d12-1bfa785ad422)

This is a simple calculator application built using Python's Tkinter library. It provides basic arithmetic operations along with additional functionalities like squaring and square root calculations.

>Features
- Basic arithmetic operations: addition, subtraction, multiplication, division.
- Squaring and square root operations.
- Clear button to reset the current and total expressions.
- Key bindings for digits, operators, and Enter key for evaluation.

>Requirements
- Python 3.x
- Tkinter (usually included with standard Python installations)

>Usage
- Digits and Decimal Point: 
Click on the digit buttons or press the corresponding keys (0-9, '.') to input numbers.

- Operators: 
Click on the operator buttons or press the corresponding keys (`/`, `*`, `-`, `+`) to perform operations.

- Special Buttons:
 C: Clear the current and total expressions.
  x²: Square the current expression.
 √x: Calculate the square root of the current expression.
  =: Evaluate the current expression and display the result.
  
- Key Bindings:
 Digits: Press keys 0-9 to input digits.
 Operators: Press keys `/`, `*`, `-`, `+` to input operators.
 Enter: Press Enter key to evaluate the current expression.

>Code Structure
- calculator.py: The main script that contains the `Calculator` class and its methods to create and manage the calculator UI.

>Main Components
1. Initialization and Setup:
   - __init__: Initializes the main window, sets its geometry, and creates frames for the display and buttons.
   - create_display_frame: Creates the frame that holds the display labels.
   - create_display_labels: Creates the labels for the total expression and current expression and packs them into the display frame.

2. Button Creation and Layout:
   - create_buttons_frame: Creates the frame that holds all the buttons.
   - create_digit_buttons: Creates digit buttons (0-9 and '.') and places them on the grid in the buttons frame.
   - create_operator_buttons: Creates operator buttons ('/', '*', '-', '+') and places them on the grid.
   - create_special_buttons: Calls methods to create special function buttons (clear, equals, square, square root).

3. Button Actions:
   - add_to_expression: Adds a digit or '.' to the current expression.
   - append_operator: Appends an operator to the current expression and updates the total expression.
   - clear: Clears both the current and total expressions.
   - square: Squares the current expression.
   - sqrt: Takes the square root of the current expression.
   - evaluate: Evaluates the total expression and updates the display with the result.

4. **Display Update**:
   - `update_total_label`: Updates the total expression label.
   - `update_label`: Updates the current expression label, limiting it to 11 characters for display.

5. Key Bindings:
   - bind_keys: Binds digit keys and operator keys to their respective actions. Also binds the return key to evaluate the expression.

6. Main Loop:
   - run: Starts the Tkinter main loop to run the application.

