# Bank Account Management System

A C++ class for representing banking functions in a simple bank management system.

## Data Dictionary

| Attribute       | Data Type      | Description                        |
|-----------------|----------------|------------------------------------|
| `accountNumber` | `std::string`  | Unique account identifier.         |
| `holderName`    | `std::string`  | Name of the account holder.        |
| `balance`       | `double`       | Current balance of the account.    |
| `type`          | `string`       | "Deposit" or "Withdrawal"          |
| `amount`        | `double`       | Amount of transaction              |
| `timestamp`     | `string`       | Time transaction took place        | 

## Method List

| Method Signature                                           | Return Type         | Description                                                                  | 
|------------------------------------------------------------|---------------------|------------------------------------------------------------------------------|
|`BankAccount()`                                             | (Constructor)       | Default constructor.                                                         |
|`BankAccount(accNum, holder, bal)`                          | (Constructor)       | Parameterized constructor.                                                   |
|`GetAccountNumber() const`                                  | `std::string`       | Gets the account's number.                                                   |
|`GetHolderName() const`                                     | `std::string`       | Gets the account holder's name.                                              |
|`GetBalance() const`                                        | `double`            | Gets the current balance on the account.                                     |
|`static void printAccount(const BankAccount &account)`      | `void`              | Prints all account information.                                              |
|`BankAccount(const BankAccount&other)`                      | `Constructor`       | Copies another BankAccount object                                            |
|`BankAccount &operator=(const BankAccount &other)`           | `BankAccount&`      | Assigns values from another BankAccount object                              |
|`virtual ~BankAccount()`                                    | `Destructor`        | For cleanup                                                                  |
|`virtual void deposit(double amount)`                       | `void`              | Add money to balance. Prints confirmation                                    |
|`virtual void withdraw(double amount)`                      | `void`              | Subtracts money from balance. Prints a confirmation or failure message       |
|`bool operator==(const BankAccount &other) const`           | `bool`              | Compares account numbers for equality                                        |                
|`bool operator<(const BankAccount &other) const`            | `bool`              | Returns true if the balance is less than the other account balance.          |
|`bool operator>(const BankAccount &other) const`            | `bool`              | Returns true if the balance is greater than the other account balance        |
|`static BankAccount createAccountFromInput()`               | `BankAccount`       | Prompts user to input account number, holder name, and initial balance.      |
|`void printHistory()`                                       | `void`              | Prints all transactions                                                      |















