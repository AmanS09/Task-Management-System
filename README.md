# Task Management System Application

## Overview

The Task Management System Application is designed to enhance productivity and organization by providing a user-friendly interface for managing tasks. This application is built using the latest version of Angular.
## Screen Shots

![Screenshot_1-7-2024_223015_angular-task-management-system-sigma vercel app](https://github.com/Mayank-Tiwari01/Angular-Task-Management-System/assets/103953234/dba4f49c-f3fa-4852-bc2e-1ea967261448)
![Screenshot_1-7-2024_1399_angular-task-management-system-sigma vercel app](https://github.com/Mayank-Tiwari01/Angular-Task-Management-System/assets/103953234/514a1547-fad1-4694-bc4c-e17e1f6d853f)
![Screenshot_1-7-2024_223245_angular-task-management-system-sigma vercel app](https://github.com/Mayank-Tiwari01/Angular-Task-Management-System/assets/103953234/b2643eb6-0849-4297-a656-ec0f304fbe52)
![Screenshot_1-7-2024_162217_localhost](https://github.com/Mayank-Tiwari01/Angular-Task-Management-System/assets/103953234/071c3e66-0d12-43d1-b84c-fd0c483708f0)
![Screenshot (590)](https://github.com/Mayank-Tiwari01/Angular-Task-Management-System/assets/103953234/d072e220-0df4-475b-9ad1-9396bc8ecf32)



## Features

### Task Management
- **Add New Tasks**: Users can create new tasks by providing a title, description, due date, and priority level (low, medium, high).
- **Update Task Status**: Tasks can be updated to reflect their current status (to-do, in-progress, completed).
- **Edit Tasks**: Users can modify existing tasks, updating any of the task details as needed.
- **Delete Tasks**: Tasks can be removed from the list.

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

