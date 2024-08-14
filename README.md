# LibraryDatabaseManagementSystem

1.
Header Files
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

These are standard header files in C. `<stdio.h>` for input and output functions, `<stdlib.h>` for dynamic memory allocation functions (`malloc`, `free`), and `<string.h>` for string manipulation functions (`strcmp`).

-------------------------------------------------
2. 
Structure Definition

struct Book {
    char title[100];
    char author[100];
    int year;
};

Defines a structure named `Book` to represent a book. It contains three members: `title` (string), `author` (string), and `year` (integer).

-------------------------------------------------
3. 
Function to Add a Book

void addBook(struct Book library[], int *numBooks) {
    // ...
}

This function allows the user to input details for a new book and adds it to the library array.

-------------------------------------------------
4. 
Function to Display Books

void displayBooks(struct Book library[], int numBooks) {
    // ...
}

This function displays details of all books in the library.

-------------------------------------------------
5. 
Function to Search for a Book

void searchBook(struct Book library[], int numBooks, char title[]) {
    // ...
}

This function searches for a book by title in the library and displays its details if found.

-------------------------------------------------
6. 
Main Function

int main() {
    // ...
}

The main function initializes the library array and variables. It then presents a menu-driven interface to the user, allowing them to choose between adding a book, displaying all books, searching for a book, or exiting the program.

-------------------------------------------------
7. 
Menu-Driven Loop

do {
    // ...
} while (choice != 4);

A do-while loop that continues to display the menu until the user chooses to exit (option 4).

-------------------------------------------------
8. 
Switch Statement

switch (choice) {
    // ...
}

Handles the user's choice by calling the appropriate function or displaying an error message for an invalid choice.

-------------------------------------------------
9. 
Exit Condition

case 4:
    printf("Exiting the program...\n");
    break;
Exits the program when the user chooses option 4.

-------------------------------------------------
10. 
Input/Output

printf("Enter your choice: ");
scanf("%d", &choice);
Prompts the user for input and stores the choice in the `choice` variable.

-------------------------------------------------
11. 
Error Handling

default:
    printf("Invalid choice. Please enter a valid option.\n");
    
Handles cases where the user enters an invalid choice.

-------------------------------------------------
12. 
Limitations

The code has some limitations, such as a fixed array size for the library (100 books) and a lack of robust error handling. In a real-world 
application, you would need to handle edge cases more carefully.

-------------------------------------------------
13. 
Structure Usage

The `struct Book` structure is used to represent each book's data, allowing for a more organized and maintainable code structure.
