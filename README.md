# Task Tracker CLI

## Overview
Task Tracker CLI is a simple command-line interface (CLI) application that allows users to manage tasks efficiently. Users can add, update, delete, and track tasks by their status (To-Do, In Progress, Done). The tasks are stored in a JSON file for persistence.

## Features
- Add new tasks with a description
- Update existing tasks
- Delete tasks
- Mark tasks as "In Progress" or "Done"
- List all tasks or filter by status
- Persistent task storage using a JSON file

## Installation
1. Clone the repository or download the script.
   ```sh
   git clone <repository-url>
   cd task_tracker
   ```
2. Ensure you have Python installed (Python 3.x recommended).
3. No external libraries are required as it uses Python's built-in modules.

## Usage
Run the script using Python and pass commands as arguments:

### Adding a Task
```sh
python task_tracker.py add "Buy groceries"
```
Output:
```
Task added successfully (ID: 1)
```

### Updating a Task
```sh
python task_tracker.py update 1 "Buy groceries and cook dinner"
```

### Deleting a Task
```sh
python task_tracker.py delete 1
```

### Marking a Task as In Progress
```sh
python task_tracker.py mark-in-progress 1
```

### Marking a Task as Done
```sh
python task_tracker.py mark-done 1
```

### Listing Tasks
```sh
python task_tracker.py list
```
To filter tasks by status:
```sh
python task_tracker.py list done
python task_tracker.py list todo
python task_tracker.py list in-progress
```

## File Structure
- `task_tracker.py` - Main CLI script
- `tasks.json` - Stores task data (auto-created if missing)

## Error Handling
- Handles invalid commands and arguments
- Prevents duplicate task IDs
- Displays meaningful error messages when tasks are not found

## Future Improvements
- Add due dates and priorities for tasks
- Implement a search feature
- Create a graphical user interface (GUI)

## License
This project is open-source and available under the MIT License.

## Contributors
Developed by [Your Name]. Contributions are welcome!

