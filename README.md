# Jupyter Notebook: ATM Machine Simulation Using OOP

## Overview
This notebook implements a simple ATM machine simulation using Python's object-oriented programming. The system includes:
- A `BankAccount` class to manage account details and transactions.
- A `User` class to represent the account holder.
- An `ATM` class to handle user interactions like checking balance, depositing, withdrawing, and transferring funds.
- The code emphasizes OOP concepts such as encapsulation, abstraction, and class relationships.
- Input validation and error handling are included for a realistic simulation.

## Explanation of OOP Concepts Used
1. **Encapsulation**: Attributes like `_balance`, `_pin`, and `_transactions` are private (indicated by the underscore), accessible only through methods. This protects the data from external modification.
2. **Abstraction**: The `ATM` class hides the complexity of transactions and authentication, providing a simple interface (menu) for the user.
3. **Class Relationships**: The `ATM` class interacts with `BankAccount` and `User` classes, demonstrating composition (ATM contains a reference to a `BankAccount`).
4. **Modularity**: Each class has a single responsibility (`User` for authentication, `BankAccount` for transactions, `ATM` for user interaction), making the code reusable and maintainable.

## How to Run
1. Copy the code into a Jupyter Notebook, separating markdown and code cells as shown.
2. Run each cell in sequence.
3. After running the final cell, interact with the ATM by entering menu choices and amounts as prompted.
4. The program will simulate ATM operations like checking balance, depositing, withdrawing, transferring, and viewing transaction history.

## Notes
- The transfer functionality uses a dummy recipient account for simplicity. In a real system, recipient accounts would be retrieved from a database.
- Error handling ensures invalid inputs (e.g., negative amounts or non-numeric inputs) are caught gracefully.
- Transaction history includes timestamps for realism.
- The code is kept simple but can be extended with features like multiple accounts, PIN retries, or a database.

