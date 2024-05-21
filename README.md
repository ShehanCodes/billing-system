# Simple Restaurant Bill Generator

## Description

This is a simple console-based application written in C that generates restaurant bills. The program allows users to input the details of ordered items, their quantities, and prices, and then calculates the total bill amount including discounts and taxes. The application can also save and retrieve past invoices.

## Features

- Add multiple items with their names, prices, and quantities.
- Calculate the subtotal, discount, service tax, and grand total.
- Save invoices to a file.
- Retrieve and display all saved invoices.
- Search for a specific customer's invoice by name.

## Requirements

- A C compiler (e.g., GCC)

## Installation

1. Clone the repository or download the source code.

    ```sh
    git clone https://github.com/yourusername/simple-restaurant-bill-generator.git
    ```

2. Navigate to the project directory.

    ```sh
    cd simple-restaurant-bill-generator
    ```

3. Compile the source code.

    ```sh
    gcc -o restaurant_bill_generator main.c
    ```

## Usage

1. Run the compiled program.

    ```sh
    ./restaurant_bill_generator
    ```

2. Follow the on-screen instructions to:
   - Generate a new invoice.
   - Show all previous invoices.
   - Search for a specific invoice by customer's name.
   - Exit the application.

### Example

```sh
$ ./restaurant_bill_generator
    ==============Jimmy's Diner==============

Please select your preferred operation

1. Generate the invoice
2. Show all the invoices
3. Search invoice
4. Exit

Your choice: 1

Please enter the name of the customer: John Doe
Please enter the number of items: 2

Please enter the item 1: Burger
Please enter the quantity: 2
Please enter the unit price: 5.99

Please enter the item 2: Soda
Please enter the quantity: 3
Please enter the unit price: 1.50

Do you want to save the invoice [y/n]: y

Successfully saved

Do you want to perform another operation? [y/n]: n

    ==============Jimmy's Diner==============

    Bye Bye :)
