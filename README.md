# Inventory Management System

**Name:** Om Kumar Singh
**Class/Section:** M
**Roll Number:** RU-26-00585
**Language:** Python 3

## Description

This is a console-based inventory management system written in Python 3. It stores items in memory and lets the user add, view, update, delete and search items. It also shows the total stock value and a low-stock report. Each item has an automatically generated ID (`I101`, `I102`, ...), a name, a quantity and a price. Items with a quantity below 5 are marked as low stock.

## Features

- Add an item with name, quantity and price (with input validation)
- View all items in a neat table
- Update the quantity or price of an item (press Enter to keep the old value)
- Delete an item by ID
- Search items by ID or name (not case sensitive)
- Total stock value (quantity × price for all items)
- Low-stock report (quantity below 5)

## Concepts Used

- Variables and data types
- Conditionals (`if`, `elif`, `else`)
- Loops (`while` and `for`)
- Functions
- Lists and dictionaries
- Error handling (`try/except`)

## Requirements

- Python 3.6 or newer
- No external libraries are needed

## How to Run

1. Make sure Python 3 is installed. Check with:
   ```bash
   python --version
   ```
2. Download or clone this repository.
3. Open a terminal in the project folder.
4. Run the program:
   ```bash
   python inventory.py
   ```
5. Choose an option from the menu and follow the prompts. Choose `0` to exit.

## Sample Input and Output

**Adding an item (Test Case 1):**

```
Choose an option: 1
Name: Pen
Quantity: 50
Price: 10
Item added.
ID: I101 | Pen | Qty: 50 | Price: 10
```

**Adding an item with an invalid quantity (Test Case 3):**

```
Choose an option: 1
Name: Pencil
Quantity: -5
Price: 4
Invalid quantity. Quantity must be a non-negative whole number. Item not added.
```

**Viewing items:**

```
------------------------------------------------------
ID      Name                     Quantity         Price
------------------------------------------------------
I101    Pen                            50            10
I102    Notebook                        3            40
------------------------------------------------------
```

**Total stock value (Test Case 4):**

```
Choose an option: 5
Total stock value: 620
```

Screenshots of all test cases are in the `images/` folder and in `Summary.md`.

## Project Structure

```
Inventory-Management-System/
├── inventory.py   # main program
├── images/        # screenshots of the test cases
├── README.md      # project description
└── Summary.md     # project summary, difficulties and solutions
```

## Notes

Items are stored only in memory, so all data is lost when the program stops.
