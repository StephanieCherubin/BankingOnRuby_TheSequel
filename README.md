# BankingOnRuby_TheSequel
This shows how to use classes, OOP, and the testing gem RSpec. #TDD
OOP and TDD will make this project remarkably simpler to tackle.

# TDD OOP TBD
_(Or how test driven development and object oriented programming were meant for each other)_

## Overview
In this session, students get first-hand experience following test-driven-development practices with professional tools like RSpec.

## Objectives
* Understand and use basic RSpec syntax (`describe`, `it`, `expect`).
* Approach projects by first outlining expectations.
* Utilize the basic building blocks of Ruby's object model including:
  * attribute (`attr_`) access methods
  * `initialize`
  * `@instance` variables and methods
  * `@@class` variables and `self.`methods

## Background
You've been approached by a small bank in a remote island nation that still uses paper to manage their six customer accounts. They don't care about security or durability. They only have a few requirements and after having a meeting to plan for the project we came up with some agile _scenarios_ describing how our BankAccount should work. Scenarios take the form of:

- Given:
- When:
- Then:

Here are the scenarios we'll be implementing today.

### Requirements

#### has a balance
- Given: a bank account
- When: it has been created
- Then: it is a bank account
    + And: it can report it's balance
    
#### making a deposit
- Given: a bank account
- When: deposit is made
- Then: it's balance increases

#### making a withdrawal
- Given: a bank account
- When: withdrawal is made
- Then: it's balance decreases

#### transferring funds
- Given: a bank account
- When: transfering funds
- Then: it's balance decreases
    + And: other account balance increases

#### minimum balance
- Given: a bank account
- When: minimum balance is set
- Then: argument error should be raised if opening balance is too low
    + And: should **NOT** raise an error if opening balance is over minimum balance
    + And: allows the bank owner to change the minimum balance

### Bonus Requirements

1. We heard that bigger banks are making lots of money with overdraft fees. Let's add an overdraft fee whenever customers overdraft their account. We should be able to change that fee for all of our accounts at any time.
1. We want to be able to see a running transaction history.

### Super Bonus Requirements

1. Power goes out quite a bit on our island nation. Bank accounts should write their transaction history to files on the disk as a backup.
1. We should be able to recover a bank account from it's transaction history file.

