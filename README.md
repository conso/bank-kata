# BANK KATA

## Outside-In ATDD

Learn and practice the double loop of Acceptance TDD. 
Get the business scenarios flowing into the Acceptance Test suite using a BDD approach.
Define acceptance criterias and use it for the outer test loop proving business correctness.

Test software modules from the outside, so defining the public interface first.

## Problem description

Create a simple bank application with the following features:

- Deposit into Account
- Withdraw from an Account
- Print a bank statement to the console

All of the methods must be void and you cannot add anymore methods to the Account class.

## Acceptance criteria

Statement should have transactions ordered from the recent to the older in the following format:

- DATE | AMOUNT | BALANCE
- date | amount | balance

The scenario for the kata is as follows:

- Given a client makes a deposit of 1000 on 29-03-2017 
- And a withdrawal of 700 on 05-04-2017 
- And a deposit of 500 on 15-04-2017 
- When she prints her bank statement 
- Then she would see a statement like the following:
DATE | AMOUNT | BALANCE
15/04/2017 | 500.00 | 800.00
05/04/2017 | -700.00 | 300.00
29/03/2017 | 1000.00 | 1000.00
