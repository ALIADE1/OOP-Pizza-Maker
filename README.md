# Pizza Factory Simulation

This C++ program simulates a simple pizza-making process using object-oriented programming concepts like inheritance and polymorphism. The program allows users to choose between different types of pizzas (Beef, Cheese, or Chicken) and follows a step-by-step pizza preparation process.

## Features

- **Encapsulation**: Uses a `Pizza` base class to define the generic pizza-making process.
- **Inheritance**: Derived classes (`ChickenPizza`, `BeefPizza`, and `CheesePizza`) override a method to specify their unique pizza type.
- **Polymorphism**: The program dynamically creates and processes the pizza type chosen by the user.
- **Dynamic Memory Management**: Uses pointers to manage derived class objects and ensure proper cleanup.

## How It Works

1. The user selects a type of pizza from the console input.
2. Based on the user's choice, a specific pizza object is created dynamically.
3. The program calls the `MakePizza` method, which:
   - Prepares the dough.
   - Adds toppings.
   - Bakes the pizza.
   - Completes the pizza-making process.
4. The dynamically allocated memory is cleaned up after use.

## Code Structure

- **Base Class (`Pizza`)**:
  - Contains the generic pizza-making process (`MakeDough`, `AddPizzaToppings`, `BakePizza`).
  - Defines a pure virtual method `GetPizzaName` for the derived classes to specify their pizza type.

- **Derived Classes**:
  - `ChickenPizza`, `BeefPizza`, and `CheesePizza` override `GetPizzaName` to return the name of the specific pizza.

- **Main Function**:
  - Accepts user input to choose a pizza type.
  - Dynamically creates the corresponding pizza object.
  - Calls the `MakePizza` method to simulate the pizza-making process.

