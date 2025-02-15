# Assignment1_SENG438 Lab Report

Lab Report #1: Intro to Testing and Defect Tracking


Group 4

Maryam 
Alison 
Svara 
Zaira

## Introduction

The objective of this lab was to enhance our knowledge of and practice exploratory,  manual, and regression testing practices. We also gained experience using the popular defect tracking system Jira. The system under test for this lab was an ATM System equipped with monetary transaction systems This system was set to be able to perform deposits, transfers between accounts and withdrawals. Furthermore the system was set up so that users could access their account with two different cards,  view their account balances as well as receipts and transaction logs.  

Prior to this lab, we had knowledge of exploratory testing, and manual scripted testing principles and practices. In exploratory testing, tests are designed and executed at the same time. While the tests are unscripted, a loose plan of what needs to be tested is beneficial to ensure comprehensive testing. Unlike exploratory testing, manual scripted testing follows a specific script as to how the system is to be tested. These tests are conducted methodically in accordance with the script. 

## High-level description of exploratory testing plan:

The following testing plan aims to evaluate the core functionalities of the ATM system to ensure that critical operations function as expected. The primary areas under test include user authentication, transactions, account handling, ATM cash management, and log and receipt generation.

### User Authentication

The system will be tested for login procedures, including valid and invalid login attempts. Scenarios involving incorrect PIN entries and account lockout conditions will be verified to ensure proper security measures are in place if a pin is entered incorrectly more than 3 times in a row.

Tests

-Valid Login: Enter correct card number and PIN.
-Invalid Card Number: Use an incorrect or non-existent card number.
-Incorrect PIN: Enter incorrect PIN multiple times.
-Locked Account Scenario: Verify behavior after multiple failed login attempts.

### Transactions

Tests will be conducted for various financial transactions, including withdrawals, deposits, fund transfers, and balance inquiries. The accuracy and consistency of these transactions will be monitored across different account types.

Tests

-Deposit valid amounts into each account.
-Verify if balance updates correctly after deposits.
-Withdraw within the available balance limit.
-Attempt to withdraw more than the available balance
-Transfer between Checking, Savings, and Money Market accounts.
-Attempt invalid transfers (e.g., transferring more than available funds).
-Verify if balances update correctly after transfers.

### Account Handling

The functionality of Checking, Savings, and Money Market accounts will be validated. The visibility of accounts depending on what card was used to access the account will be tested. 

Tests

-Check balances for Checking, Savings, and Money Market accounts.
-Verify balance remains unchanged after viewing.

###ATM Cash Handling

Cash dispensing and deposit mechanisms will be tested to ensure the ATM correctly manages available funds and that the total available balance updates correctly. 

Tests

-Check to see if the atm availability balance correctly updates after a deposit and withdrawal is made.
-Check to see if atm availability balance remains the same after a transfer of funds between accounts is made

###Logs and Receipt Testing

The system’s ability to generate accurate transaction logs and printed receipts will be evaluated. The logs should reflect all transactions accurately, and receipts must include relevant details without exposing sensitive pin information.

Test

-View logs and receipts after a transfer is made between savings and checking accounts. 

##Comparison of exploratory & manual functional testing:

Need to include a defect report generated by the bug tracking system

##Notes/discussion of peer reviews of defect reports:

Refer to the Jira report 

##How pair testing was managed, how teamwork/effort was divided:

-The group was split into 2 pairs, with each pair handling one of the testing types.
--Exploratory testing was done by Alison Gartner and Svara Patel. Both Alison and Svara conducted exploratory tests based on the script they wrote collectivly. All failed tests were reported by both parties. 
-Manual functional testing was done by Zaira Ramji and Maryam Alsayed. Both members were assigned 20 tests to conduct on the system side-by-side. Any failed tests were confirmed by both group members on both machines. ---Both group members reported the bugs they found. This process was then repeated with version 1.1 of the system.

##Difficulties encountered, challenges overcome, lessons learned:
-Difficulty: ensuring the system testing was exhaustive (exploratory)
-Challenges: ensuring we knew how to recreate bugs found
-Lesson: conduct tests more systematically and go in with a game plan (manual)

##Comments/feedback on the lab and lab document itself: 
-Would help if the system details were more thorough as it was difficult to differentiate between a feature and a bug. For example, a card is confiscated after 3 incorrect pin attempts, it seems to be a feature but it --is not stated as one so causes confusion in whether to classify it as a bug or not.
-Manual functional testing table could also be more thorough as it was occasionally difficult to discern what the inputs were supposed to be to properly conduct the tests



