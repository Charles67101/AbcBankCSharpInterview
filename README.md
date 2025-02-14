Programming Test
========

Instructions
------------

There are several deliberate design, code quality and test issues that should be identified and resolved. The section below details what the behavior of the application is supposed to be, which may not match up with how the code is currently functioning.

* Fix broken (non-passing), incorrect, or incomplete tests.
* Refactor and add features (from the section below) as you see fit; there is no need to add all the features in order to "complete" the exercise. Keep in mind that code quality is the critical measure and there should be an obvious focus on testing.
* Treat this code as if you owned this application, do whatever you feel is necessary to make this your own. *Clarification:* Please do not change the testing framework.
* In order to work on this take a fork into your own GitHub area; make whatever changes you feel are necessary and when you are satisfied submit back via a pull request. See details on GitHub's [Fork & Pull](https://help.github.com/articles/using-pull-requests) model.
* You're welcome to spend as much time as you like; however it's anticipated that this should take about 2 hours.

Application
-----------

A dummy application for a bank; should provide various functions of a retail bank.

Application is designed for Visual Studio 2017 or newer, MSTest as the testing framework (integrated into Visual Studio), and uses the .NET Framework v4.7.2. The solution is compatible with the community version.

### Current Features

* A customer can open an account.
* A customer can deposit / withdraw funds from an account.
* A customer can request a statement that shows transactions and totals for each of their accounts.
* Different accounts have interest calculated in different ways:
  * **Checking accounts** have a flat rate of 0.1%.
  * **Savings accounts** have a rate of 0.1% for the first $1,000 then 0.2%.
  * **Maxi-Savings accounts** have a rate of 2% for the first $1,000 then 5% for the next $1,000 then 10%.
* A bank manager can get a report showing the list of customers and how many accounts they have.
* A bank manager can get a report showing the total interest paid by the bank on all accounts.

### Additional Features

* A customer can transfer between their accounts.
* Change **Maxi-Savings accounts** to have an interest rate of 5% assuming no withdrawals in the past 10 days otherwise 0.1%.
* Interest rates should accrue daily including weekends, rates above are per-annum (for each year).
