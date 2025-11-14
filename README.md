This repository contains a Strong Password Checker implemented in C++ that evaluates and ensures the strength of a given password based on specific security criteria. The program efficiently validates password strength while optimizing for various constraints, such as minimum length, character diversity, and repetitive sequences.

Features
Password Validation: Ensures compliance with the following rules:

Minimum length of 6 characters.
Maximum length of 20 characters.
Includes at least one uppercase letter, one lowercase letter, and one digit.
Avoids sequences of three or more repeated characters.
Optimized Handling:

Dynamically balances replacements, insertions, and deletions to make passwords valid.
Handles edge cases for passwords that are too short or too long efficiently.
Modern C++ Implementation:

Utilizes features like the C++ ranges library and lambda functions for clean, readable, and efficient code.
Usage
Clone the Repository

bash
Copy code
git clone https://github.com/your-username/strong-password-checker.git
cd strong-password-checker
Build the Program
Use a C++ compiler (e.g., g++):


g++ -std=c++20 -o password_checker password_checker.cpp
Run the Program
Execute the compiled binary and input passwords to check:

bash
Copy code
./password_checker
Code Explanation
The core logic of the password checker consists of:

Missing Character Check: Validates the presence of uppercase, lowercase, and numeric characters using the getMissing function.
Repetition Handling: Detects and optimizes replacements for sequences of three or more repeated characters.
Length Adjustments:
Adds characters for passwords shorter than 6.
Removes characters for passwords longer than 20, minimizing necessary replacements.
Example
Input:
makefile
Password: aaa111  
Output:
Steps required to make password strong: 2  

