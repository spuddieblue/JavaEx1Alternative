# Java Program: Dice Game - Counting Doubles

### **Objective:**
Write a Java program that simulates a dice game. The program will ask the user how many times they want to roll two dice, simulate the rolls, and keep track of how many times the dice show the same number (doubles).

### **Detailed Requirements:**

1. **Introduction:**
   - The program should display an introduction explaining the purpose of the game:
     - It rolls two dice a specified number of times.
     - It tracks how many times "doubles" (both dice showing the same number) occur.

2. **Inputs:**
   - The user will input an integer indicating how many times the dice should be rolled.

3. **Processing:**
   - Use a `Random` object to generate random numbers between 1 and 6 (inclusive) for each die.
   - Roll the dice for the specified number of times, and for each roll:
     - Print the values of both dice.
     - Check if the dice show the same number (doubles).
     - If doubles are rolled, increment a counter to track the total number of doubles.

4. **Outputs:**
   - For each roll, display:
     - The roll number.
     - The values of Dice 1 and Dice 2.
     - Whether the roll resulted in doubles (e.g., `Doubles!`).
   - After all rolls, display the total number of doubles rolled.

5. **Implementation Details:**
   - Use a `Scanner` object to collect input from the user.
   - Use a `for` loop to perform the specified number of dice rolls.
   - Use the `Random` class to simulate rolling the dice.
   - Ensure the program displays a clear and user-friendly output.
   - Close the `Scanner` object at the end of the program to prevent resource leaks.

### **Example Execution:**
Welcome to the Dice Game! This game rolls two dice and keeps track of how many times you roll doubles (when both dice show the same number)

How many times do you want to roll? 5

Roll 1: Dice 1 = 3, Dice 2 = 5 Roll 2: Dice 1 = 4, Dice 2 = 4 (Doubles!) Roll 3: Dice 1 = 2, Dice 2 = 6 Roll 4: Dice 1 = 1, Dice 2 = 1 (Doubles!) Roll 5: Dice 1 = 5, Dice 2 = 3

You rolled doubles 2 times

markdown
Copy code

### **Edge Cases to Consider:**
- If the user enters `0`, no rolls should occur, and the program should simply display that no doubles were rolled.
- If a very large number is entered, ensure the program performs efficiently without errors.

### **Expected Learning Outcomes:**
- Practice using loops (`for`) to perform repetitive tasks.
- Learn to use the `Random` class to generate random numbers.
- Implement conditional logic to check for specific outcomes (e.g., doubles).
- Understand input/output operations in Java using `Scanner` and `System.out.println`.
