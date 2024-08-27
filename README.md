# Task Management System Application

## Overview

The Task Management System Application is designed to enhance productivity and organization by providing a user-friendly interface for managing tasks. This application is built using the latest version of Angular.
## Screen Shots




## Features

### Add New Tasks:
-Users can create new tasks with a title, description, due date, and priority level (Low, Medium, High).
-User-friendly form to enter task details.

### Task Management
-Update task status (To-Do, In-Progress, Completed).
-Edit task details such as title, description, due date, and priority level.
-Delete tasks from the list.


### Task Display and Sorting
- **List View**: Tasks are displayed in a list format for easy viewing.
- **Sorting**: Tasks are sorted: High > medium > low.
### Responsive Design
- **Mobile and Desktop Support**: The application is fully responsive and works well on various screen sizes, providing a consistent user experience across devices.

### Export Functionality
- **Export to CSV**: Users can export their tasks to a CSV file for external use and backup.

### History Log
- **Task History**: A detailed history log is maintained for each task, recording all changes such as creation, status updates, and edits.

## Development Details

### Technology Stack
- **Frontend**: Angular (latest version)
- **Data Persistence**: Local storage

### Project Setup

1. **Clone the Repository**:
    ```bash
    git clone <https://github.com/Mayank-Tiwari01/Angular-Task-Management-System.git>
    cd Angular-Task-Management-System
    ```

2. **Install Dependencies**:
    ```bash
    npm install
    ```

3. **Run the Application**:
    ```bash
    ng serve
    ```

    The application will be available at `http://localhost:4200/` (or you may give a custom port).

### Project Structure

- **src/app**:
  - **components**:
    - **task-form**: Handles the creation and editing of tasks.
    - **task-list**: Displays the list of tasks and sorting options.
    - **task-details**: Shows detailed information and history of a selected task.
  - **models**:
    - **task.model.ts**: Defines the Task interface.
  - **services**:
    - **task.service.ts**: Provides task management functionalities.
  - **store**:
    - **reducers**: Manages application state using ngrx store.
    - **actions**: Defines actions for state management.
    - **effects**: Handles side effects in state management.

### Detailed Features

#### Task Form Component (`task-form.component.ts` and `task-form.component.html`)
- Allows users to add and edit tasks.
- Validates input fields to ensure required information is provided.
- Maintains a history log for each task, recording changes with descriptive messages.

#### Task List Component (`task-list.component.ts` and `task-list.component.html`)
- Displays tasks in a list view.
- Provides sorting functionality to organize tasks by due date, priority, or status.

#### Task Details Component (`task-details.component.ts` and `task-details.component.html`)
- Displays detailed information about a selected task.
- Shows a history log of all changes made to the task.
- Includes icons and CSS styling for a professional and user-friendly appearance.
- 
### Data Persistence
- **Local Storage**: Ensures that task data is persisted across sessions, allowing users to retain their tasks even after refreshing the browser or closing the application.

