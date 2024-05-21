Simple Restaurant Bill Generator

Description

This is a simple console-based application written in C that generates restaurant bills. The program allows users to input the details of ordered items, their quantities, and prices, and then calculates the total bill amount including discounts and taxes. The application can also save and retrieve past invoices.

Features

Add multiple items with their names, prices, and quantities.
Calculate the subtotal, discount, service tax, and grand total.
Save invoices to a file.
Retrieve and display all saved invoices.
Search for a specific customer's invoice by name.
Requirements

A C compiler (e.g., GCC)
Installation

Clone the repository or download the source code.

sh
Copy code
git clone https://github.com/yourusername/simple-restaurant-bill-generator.git
Navigate to the project directory.

sh
Copy code
cd simple-restaurant-bill-generator
Compile the source code.

sh
Copy code
gcc -o restaurant_bill_generator main.c
Usage

Run the compiled program.

sh
Copy code
./restaurant_bill_generator
Follow the on-screen instructions to:

Generate a new invoice.
Show all previous invoices.
Search for a specific invoice by customer's name.
Exit the application.
Example
sh
Copy code
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
Code Overview

Structs
struct items: Stores item name, price, and quantity.
struct orders: Stores customer name, date, number of items, and an array of struct items.
Functions
void generateBillHeader(char name[50], char date[30]): Generates the bill header.
void generateBillBody(char item[30], int qty, float price): Generates the bill body for each item.
void generateBillFooter(float total): Generates the bill footer including discounts and taxes.
Main Workflow
The main menu is displayed with options to generate an invoice, show all invoices, search for an invoice, or exit.
Depending on the user's choice, the program will perform the selected operation.
When generating an invoice, the user inputs customer details and item details. The bill is calculated and displayed.
Invoices can be saved to a file and retrieved later.
