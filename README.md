# Bank Tech Test

### Requirements
* Deposits, withdrawal
* Account statement (date, amount, balance)
* Statement printing

### Acceptance criteria

**Given** a client makes a deposit of 1000 on 10-01-2012  
**And** a deposit of 2000 on 13-01-2012  
**And** a withdrawal of 500 on 14-01-2012  
**When** she prints her bank statement  
**Then** she would see  


```
date || credit || debit || balance
14/01/2012 || || 500.00 || 2500.00
13/01/2012 || 2000.00 || || 3000.00
10/01/2012 || 1000.00 || || 1000.00
```
How to use:

```
$ git clone https://github.com/vickymg/bank_tech_test.git
$ cd bank_tech_test
$ bundle
```
To run tests:
```
$ rspec
```

To run the program in IRB:
```
$ irb
> require './lib/bank.rb'
> bank = Bank.new
> bank.deposit(100, "01/06/2016")
> bank.deposit(100, "02/06/2016")
> bank.withdraw(50, "03/06/2016")
> bank.print_statement
```
