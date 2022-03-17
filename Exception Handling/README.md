## EXCEPTION HANDLING IN PYTHON
An __exception__ is an error which happens at the time of execution of a program. However, while running a program, Python generates an exception that should be handled to avoid your program to crash. In Python language, exceptions trigger automatically on errors, or they can be triggered and intercepted by your code.

**Syntax Error:**  As the name suggests this error is caused by the wrong syntax in the code. It leads to the termination of the program.

**Exceptions:**  Exceptions are raised when the program is syntactically correct, but the code resulted in an error. This error does not stop the execution of the program, however, it changes the normal flow of the program.

**Try and Except Statement – Catching Exceptions:**  Try and except statements are used to catch and handle exceptions in Python. Statements that can raise exceptions are kept inside the try clause and the statements that handle the exception are written inside except clause.

## ATM PIN Change - Case Study
> **Problem Statement:** The cast of `The Big Bang Theory` sitcom have their bank accounts in our State Bank of India and Dr. Sheldon Cooper wishes to change his ATM PIN. There are 4 different ways one can do that:
>- via ATM machine
>- via IVRS Service (Interactive Voice Response Service)
>- via Internet Banking 
>- via SMS Service
>
> Write an interactive program to implement the above 4 methods with the help of DataFrames, Functions, Exeception Handling, APIs and anything necessary. 

The `ATM_PIN_CHANGE.ipynb` program covers all the 4 methods as precisely as possible to the actual procedure of PIN change. 
In order to change your PIN, it is necessary to physically visit the nearest ATM for security purposes. Keeping that in mind, the SMS service, Internet Banking, and the IVRS call service generate an OTP  authentication and the person should visit the nearest ATM with the received OTP and opt for a PIN change option.

1. **ATM PIN Change procedure:**
- Step 1: Insert the card and select PIN change option.
- Step 2: Click on 'Yes' if you already have an OTP, else click 'No'.
- Step 3: An 6-digit OTP will be sent to the registered mobile number.
- Step 4: Enter the 6-digit OTP
- Step 5: Enter your new PIN.
2. **IVRS Service:**
- Step 1: Enter the last 5 digits of your Account Number.
- Step 2: Enter the last 5 digits of your Debit Card Number.
- Step 3: An 6-digit OTP will be sent to the registered mobile number.
- Step 4: Visit the nearest ATM.
3. **Internet Banking:**
- Step 1: Log into the account with your User ID and Password.
- Step 2: Navigate to e-services > ATM Card Services > ATM PIN Generation. (This is assumed to already be done in our program)
- Step 3: An 6-digit OTP will be sent to the registered mobile number.
- Step 4: Visit the nearest ATM.
4. **SMS Service:**
- Step 1: From the registered mobile number, send an SMS to 567676 using the format PIN XXXX YYYY
- Step 2: Here XXXX denotes the last four digits of the SBI ATM card while YYYY denotes the last four digits of SBI Account Number.
- Step 3: An 6-digit OTP will be sent to the registered mobile number.
- Step 4: Visit the nearest ATM.

### Endnotes:
The program depicts the use of functions and exception handling in Python, Indexing in Pandas, and the use of Twilio API. There is much room for improvement in the code, like we can add more functionalities in the ATM class such as Balance enquiry, Withdrawal, User authentication etc. 
