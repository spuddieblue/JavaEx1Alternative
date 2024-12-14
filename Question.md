# Java Program: Workout Tracker

### **Objective:**
Write a Java program that serves as a workout tracker for users. The program allows users to log their workouts, view their workout history, and provides a summary of their workout statistics.

---

### **Detailed Requirements:**

#### **1. Functionality Overview:**
- The program keeps a record of workouts for each user in a text file.
- It allows users to:
  - Add new workouts.
  - View workout history.
  - Exit the program.

---

#### **2. Features:**

##### **a. User Management:**
- Each user is identified by a username.
- Workout records are saved in a dedicated file named `<username>_workouts.txt` inside a `users` folder.
- If the user is new, the program creates a file for them. If the user already exists, it welcomes them back and loads their workout history.

##### **b. Adding Workouts:**
- Users can log exercises with the type of activity and amount:
  - If the exercise is running (contains "run"), the amount is logged in minutes.
  - For all other exercises, the amount is logged in reps.

##### **c. Viewing Workouts:**
- Users can view their workout history by reading the saved file.

##### **d. Workout Summary:**
- At the end of the session, the program provides an analysis of the user's workout history, including:
  - Total workouts completed.
  - Total reps and minutes across all workouts.
  - Highest reps in one workout.
  - Longest workout in minutes.
  - Average reps and minutes per workout.

---

#### **3. Inputs:**
- **Username**: A unique string identifying the user.
- **Exercise Details**:
  - Name of the exercise.
  - Amount of reps (or minutes if it's running).
- **Menu Choice**:
  - `1` for adding workouts.
  - `2` for viewing workouts.
  - `3` to exit the program.

---

#### **4. Outputs:**
- Welcome message (new or returning user).
- Workout history (when viewed).
- Confirmation message when a workout is logged.
- Final workout summary, including:
  - Total workouts.
  - Total reps and minutes.
  - Maximum reps and longest workout.
  - Average reps and minutes per workout.

---

### **Example Execution:**

#### **Session Start:**
=== Workout Tracker === Enter username: JohnDoe Welcome back, JohnDoe! Loading your workout history...

=== JohnDoe's Workout Tracker ===

Add Workout
View Workouts
Exit
Choice: 1 Enter exercise: Push-ups Enter number of reps/minutes: 30 Workout saved to your log!

=== JohnDoe's Workout Tracker ===

Add Workout
View Workouts
Exit
Choice: 2

Your Workout History: Push-ups: 30 reps Running: 20 minutes Pull-ups: 15 reps

markdown
Copy code

#### **Session Summary:**
=== JohnDoe's Workout Summary === Total workouts completed: 3 Total reps across all exercises: 45 Total minutes across all exercises: 20 Highest reps in one workout: 30 Longest workout (in minutes): 20 Average reps per workout: 15.00 Average minutes per workout: 6.67

Keep up the good work, JohnDoe!

markdown
Copy code

---

### **Edge Cases to Consider:**
- **New User**: Ensure the program creates a new file and does not crash if the user's file does not exist.
- **No Workouts Logged**: Handle cases where a user views the summary without logging any workouts.
- **Case Insensitivity**: Ensure usernames and exercises are treated in a case-insensitive manner (e.g., `Running` and `running` should be considered the same).

---

### **Implementation Details:**
- Use the `Scanner` class for user input and the `File` class for managing user files.
- Log workouts using `FileWriter` and `PrintWriter` to append data to the user's file.
- Read workout history using a `Scanner` object with the user's file.
- Perform analysis on the workout file by parsing the stored data.

---

### **Expected Learning Outcomes:**
- Understand file handling in Java (`File`, `FileWriter`, `PrintWriter`, `Scanner`).
- Work with loops (`do-while`) for menu-driven programs.
- Develop modular programs with conditional logic (`if-else`).
- Learn how to calculate and display summary statistics from stored data.
- Practice user-friendly input/output handling.
