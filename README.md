# Calculator_App
The Calculator App is a Java application that provides a graphical user interface (GUI) for performing basic arithmetic calculations. It uses Swing components for the GUI and includes features such as number input, arithmetic operations, and result display.


# Files
1. CalculatorApp.java: This file contains the main class CalculatorApp, which serves as the entry point for the application. It creates an instance of the CalculatorGui class and makes the GUI visible.
2. CalculatorGui.java: This file contains the CalculatorGui class, which extends JFrame and represents the main GUI window of the application. It sets up the GUI components, including a display field for showing the numbers and results, and buttons for number input and arithmetic operations. It also handles button click events to perform the calculations.
3. CalculatorService.java: This file contains the CalculatorService class, which provides the actual arithmetic calculations for the application. It includes methods for addition, subtraction, multiplication, and division.
4. CommonConstants.java: This file contains the CommonConstants class, which defines common constants used in the application, such as the application name, the size of the GUI window, and the configurations for the display field and buttons.


# Usage
To use the Calculator App, follow these steps:

1. Compile the Java files:
   ```bash
    javac CalculatorApp.java CalculatorGui.java CalculatorService.java CommonConstants.java
   ```
2. Run the compiled Java program: java CalculatorApp
   ```bash
   java CalculatorApp
   ``` 
3. The Calculator App GUI window will appear. You can enter numbers and perform arithmetic operations using the buttons.
4. To enter numbers, click the respective number buttons (0-9).
5. To perform arithmetic operations, click the corresponding operator buttons (+, -, x, /). The current number in the display field will be used as the first operand.
6. To calculate the result, click the "=" button. The result will be displayed in the display field.


## Class Details

### 1. CalculatorApp.java
- **Description:** This class serves as the entry point for the application.
- **Methods:**
  - `main(String[] args)`: Creates an instance of `CalculatorGui` and displays the GUI.

### 2. CalculatorGui.java
- **Description:** Represents the main GUI window of the application.
- **Constructors:**
  - `CalculatorGui()`: Initializes the JFrame with the application name, size, and close operation, and sets up GUI components.
- **Methods:**
  - `addGuiComponents()`: Sets up GUI components including display field and buttons, and handles layout and event handling.
  - `getButtonLabel(int buttonIndex)`: Returns the label for buttons based on index.
  - `actionPerformed(ActionEvent e)`: Handles button click events and performs arithmetic calculations.

### 3. CalculatorService.java
- **Description:** Provides arithmetic calculations for the application.
- **Methods:**
  - `setMathSymbol(char mathSymbol)`: Sets the mathematical symbol for the operation.
  - `setNum1(double num1)`: Sets the first operand.
  - `setNum2(double num2)`: Sets the second operand.
  - `add()`, `subtract()`, `multiply()`, `divide()`: Perform corresponding arithmetic operations and return the result.

### 4. CommonConstants.java
- **Description:** Contains common constants used in the application.
- **Constants:**
  - Various constants for application name, GUI size, text field properties, button grid layout, and font sizes.

This set of classes represents a basic calculator application with a GUI interface for performing arithmetic operations.
