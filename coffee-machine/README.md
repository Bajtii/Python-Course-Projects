# ☕ Coffee Machine Simulator (OOP in Python)

This project simulates a basic coffee vending machine using **Object-Oriented Programming (OOP)** principles in Python. It handles drink selection, resource tracking, payment processing, and order fulfillment via console interaction.

---

## 📦 Project Structure

The system is composed of four main classes:

- `CoffeeMaker` – manages water, milk, and coffee levels
- `MenuItem` – defines individual drink recipes
- `Menu` – stores and retrieves available drinks
- `MoneyMachine` – handles payment via virtual coins

---

## 🧠 Program Flow

1. Show menu: `espresso/latte/cappuccino`
2. Accept user input (`drink name`, `report`, or `off`)
3. If drink selected:
   - Check ingredient sufficiency
   - Process virtual coin payment
   - If successful → make coffee

---

## 🧰 Class Descriptions

### `CoffeeMaker`
Manages internal resource levels and coffee brewing logic.

```python
class CoffeeMaker:
    def report(self):
        """Prints current water, milk, and coffee levels."""

    def is_resource_sufficient(self, drink):
        """Checks if enough ingredients are available for the drink."""

    def make_coffee(self, order):
        """Deducts required ingredients and confirms the coffee is made."""
```
### `MenuItem`

```python
class MenuItem:
    def __init__(self, name, water, milk, coffee, cost):
        self.name = name                # e.g. "latte"
        self.cost = cost                # price in dollars
        self.ingredients = {
            "water": water,
            "milk": milk,
            "coffee": coffee
        }
```

### `Menu`

```python
class MoneyMachine:
    def report(self):
        """Displays current profit."""

    def process_coins(self):
        """Asks the user to input coin quantities and returns the total amount."""

    def make_payment(self, cost):
        """
        Returns True if payment is sufficient.
        Deducts cost and returns change if needed.
        """
```

### `MoneyMachine`

```
class MoneyMachine:
    def report(self):
        """Displays current profit."""

    def process_coins(self):
        """Asks the user to input coin quantities and returns the total amount."""

    def make_payment(self, cost):
        """
        Returns True if payment is sufficient.
        Deducts cost and returns change if needed.
        """

```
💰 Accepted coins: quarters (0.25), dimes (0.10), nickles (0.05), pennies (0.01)


