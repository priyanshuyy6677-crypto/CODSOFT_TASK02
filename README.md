# 🧮 Simple Calculator – C++

A simple **console-based calculator program** developed in C++. This project allows the user to enter two numbers and choose an arithmetic operation to calculate the result.

## 📌 Features

* ➕ Addition
* ➖ Subtraction
* ✖️ Multiplication
* ➗ Division
* ⚠️ Handles division by zero
* 🔢 Supports decimal numbers
* 💻 Easy-to-use console interface

## 🛠️ Technologies Used

* **Language:** C++
* **Library:** `<iostream>`
* **Concepts:** `switch-case`, arithmetic operators, conditional statements, user input/output

## 💻 Source Code

```cpp
#include <iostream>
using namespace std;

int main() {
    double num1, num2;
    char operation;

    cout << "===== Simple Calculator =====" << endl;

    cout << "Enter first number: ";
    cin >> num1;

    cout << "Enter an operation (+, -, *, /): ";
    cin >> operation;

    cout << "Enter second number: ";
    cin >> num2;

    switch (operation) {
        case '+':
            cout << "Result = " << num1 + num2 << endl;
            break;

        case '-':
            cout << "Result = " << num1 - num2 << endl;
            break;

        case '*':
            cout << "Result = " << num1 * num2 << endl;
            break;

        case '/':
            if (num2 != 0)
                cout << "Result = " << num1 / num2 << endl;
            else
                cout << "Error: Division by zero is not allowed." << endl;
            break;

        default:
            cout << "Invalid operation!" << endl;
    }

    return 0;
}
```

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/simple-calculator-cpp.git
```

### 2. Open the project folder

```bash
cd simple-calculator-cpp
```

### 3. Compile the program

```bash
g++ main.cpp -o calculator
```

### 4. Run the program

**Windows:**

```bash
calculator.exe
```

**Linux/macOS:**

```bash
./calculator
```

## 🖥️ Sample Output

```text
===== Simple Calculator =====
Enter first number: 25
Enter an operation (+, -, *, /): *
Enter second number: 4
Result = 100
```

## 📚 Learning Outcomes

This project helped me practice:

* C++ fundamentals
* Arithmetic operations
* `switch-case` statements
* Conditional statements
* User input and output
* Basic error handling
* Writing interactive console programs

## 🚀 Future Improvements

* Add modulus operation (`%`)
* Add a menu-based interface
* Allow multiple calculations without restarting
* Add advanced mathematical operations
* Improve input validation

## 👩‍💻 Author

**priyaanshu yadav**

This project was developed as part of my **C++ programming practice/internship tasks**.

---

⭐ If you found this project useful, consider giving the repository a star!
