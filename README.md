# ATM CONSOLE BASED USING PYTHON 

This Python program simulates an **ATM** system with a simple console-based interface. The system provides various functionalities, such as withdrawing funds, depositing money, generating and verifying PINs, and retrieving mini statements. It uses a dictionary to store account information and demonstrates basic Python concepts like loops, conditionals, and data structures.

## Features

1. **Withdrawal**: 
   - Users can withdraw money from their account.
   - The program validates if the entered PIN is correct.
   - It also checks whether the account has sufficient funds before processing the withdrawal.

2. **Deposit**:
   - Users can deposit money into their accounts.
   - The deposited amount is added to the user's balance.

3. **Pin Generation**:
   - If a user’s account doesn’t have a PIN, they can generate one.
   - If a PIN already exists, the system prevents users from generating a new one and prompts them with an appropriate message.

4. **Mini Statement**:
   - Users can view their account details, such as their name, account number, date of birth, and balance.
   - The program ensures the user enters the correct PIN before allowing access to the mini statement.

5. **Account Validation**:
   - Each operation checks if the account number entered by the user exists in the system.
   - If the account doesn’t exist, the system notifies the user.

6. **Simple Menu-driven Interface**:
   - The program uses a loop to display a simple menu of options, which repeats until the user decides to exit.

## How It Works

1. **Account Structure**:
   - Accounts are stored in a dictionary where each key represents an account number.
   - Each account contains:
     - Name of the account holder
     - Date of birth in `dd-mm-yyyy` format
     - Current account balance
     - Pin number (or `None` if not set)

2. **Menu Options**:
   - **Option 1: Withdrawal**: The user is prompted to enter their account number and PIN. If the account exists and the PIN is correct, they can withdraw a specified amount. The system checks if there are enough funds to complete the transaction.
   
   - **Option 2: Deposit**: The user is asked for their account number and the deposit amount. The system adds the specified amount to the user’s account balance.

   - **Option 3: Pin Generation**: If the user doesn't already have a PIN, they can create one by entering it twice for confirmation. If a PIN is already set for the account, the system will notify the user and prevent pin generation.

   - **Option 4: Mini Statement**: The user must enter the correct account number and PIN to access their account's mini statement. The statement includes details such as the account holder's name, account number, date of birth, and current balance.

   - **Option 5: Exit**: Exits the program.

3. **Input Validation**:
   - The program checks for invalid inputs, such as incorrect account numbers or PINs, and informs the user appropriately.

### Example Scenarios:

1. **Option 1 - Withdrawal**:
   - The user enters their account number and PIN, followed by the amount to withdraw. The system checks for sufficient funds and completes the withdrawal if everything is valid.

2. **Option 2 - Deposit**:
   - The user enters their account number and the deposit amount. The system updates the balance accordingly.

3. **Option 3 - Pin Generation**:
   - The user enters a new PIN and confirms it. The system then saves the new PIN for the account.
   
4. **Option 4 - Mini Statement**:
   - The user enters their account number and PIN. If the PIN matches, the system displays their account information, including name, account number, date of birth, and balance.

## Additional Notes

- This project is a simple console-based ATM simulation. For production systems or more complex simulations, you could integrate a GUI, a database, or implement features like password encryption.
- This program does not persist data between sessions. Once the program is closed, all account data is reset. You can modify the code to save data in a file or a database if needed.
