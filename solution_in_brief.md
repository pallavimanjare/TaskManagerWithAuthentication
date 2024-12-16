# Task Manager with User Authentication and Task Management Features

## High-Level Overview

### 1. User Authentication

#### Registration
- **Function**: `register_user()`
- **Steps**:
  - Prompt the user to enter a username and password.
  - Check if the username is unique.
  - Hash the password for security.
  - Store the username and hashed password in a file.

#### Login
- **Function**: `login_user()`
- **Steps**:
  - Prompt the user for their username and password.
  - Validate the credentials by comparing them with the stored data.
  - Grant access to the task manager upon successful login.

### 2. Task Management

#### Add a Task
- **Function**: `add_task()`
- **Steps**:
  - Prompt the user for a task description.
  - Assign a unique task ID and set the status to Pending.
  - Store the task in a file.
  - Confirm that the task was added.

#### View Tasks
- **Function**: `view_tasks()`
- **Steps**:
  - Retrieve and display all tasks for the logged-in user.
  - Show the task ID, description, and status (Pending or Completed).

#### Mark a Task as Completed
- **Function**: `mark_task_completed()`
- **Steps**:
  - Allow the user to select a task by its ID.
  - Update its status to Completed.

#### Delete a Task
- **Function**: `delete_task()`
- **Steps**:
  - Allow the user to select a task by its ID.
  - Delete it from their task list.

### 3. Interactive Menu
- **Function**: `menu()`
- **Steps**:
  - Display options: Add a Task, View Tasks, Mark a Task as Completed, Delete a Task, Logout.
  - Call the corresponding function based on user choice.
  - Loop back to the menu until the user logs out.

### 4. Budget Management (Optional)

#### Set and Track Budget
- **Function**: `set_budget()`, `track_budget()`
- **Steps**:
  - Input a monthly budget.
  - Calculate total expenses and compare with the budget.
  - Display warnings or remaining balance.

#### Save and Load Expenses
- **Function**: `save_expenses()`, `load_expenses()`
- **Steps**:
  - Save expenses to a CSV file.
  - Load expenses from the CSV file on program start.

#### Interactive Menu
- **Function**: `budget_menu()`
- **Steps**:
  - Display options: Add Expense, View Expenses, Track Budget, Save Expenses, Exit.
  - Implement conditions for each menu selection.
