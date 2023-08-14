# ATM Dispenser

## Problem

Develop a program that simulates the delivery of bills when a customer makes a withdrawal at an ATM. The basic requirements are as follows:
- Deliver the smallest number of bills;
- It is possible to withdraw the requested amount with the banknotes available;
- Infinite customer balance;
- Available banknotes of $100; $50; $20 and $10

## Solution

The Chain of Responsibility pattern has been used to avoid coupling the sender of the request to the receiver and gives more than one receiver object the opportunity to handle the request.

Each subclass defines the value of the Currency through ```getDispenserValue()```. If a specific dispenser needs to have its own business logic, just need to implement the method ```dispense()```.

<img width="897" alt="atm-diagram" src="https://github.com/kelciocajueiro/atm-dispenser/assets/1596545/aaa1d3f3-b068-40a7-838d-ab4897447d65">


## Running the code

```
git clone https://github.com/kelciocajueiro/atm-dispenser.git
cd ../atm-dispenser/src
javac com/example/*.java
java com.example.Main
```

## Result

<img width="385" alt="atm-main" src="https://github.com/kelciocajueiro/atm-dispenser/assets/1596545/4f1656c7-43e9-4815-9d8e-34f9bf7831c6">
