📝 Enhanced ToDo List Application
Project Description
This project is a task management web application (ToDo List) developed with React and TypeScript. It serves as a solid foundation for mastering React fundamentals, including state management, multi-page navigation (routing), and interaction with the browser's local storage.

The application simulates a complete environment with:

Simple user authentication.

Protected navigation.

Full CRUD operations on tasks (Create, Read, Update, Delete).

A modern design based on a Blue/Green/White color palette.

🚀 Key Features
This project integrates several functional and User Experience (UX) improvements:

Feature,Description

Add Task,Creates a new task with text.

Edit Task,Allows modification of both the text and the completion status of an existing task.

Delete Task,Removes a task from the list.

State Toggle,"Marks a task as ""Active"" or ""Completed"" via a checkbox.

Completion Option,"Allows specifying a task as ""completed"" directly upon creation through the form.

User Experience and State Management
Task Persistence: Tasks are stored in the browser's localStorage. They are not lost when the user refreshes the application.

Dynamic Filters: Allows filtering the displayed task list by three states: All, Active, or Completed.

Task Counters: Displays the total number of tasks in real-time, as well as the count for active and completed tasks.

Quick Clean-up: A "Clear Completed" button that allows deleting all finished tasks in a single click.

Security and Navigation
Simple Authentication (Mock): Managed by a local state (isLoggedIn and username). The user must log in to access the task list.

Protected Navigation: Uses React Router and <Navigate /> components to redirect unauthenticated users to the login page (/login).

Authentication Persistence: The user's login status is stored in localStorage, allowing them to remain logged in even after refreshing the browser page.

🧱 Project Architecture
The project is organized following a classic modular React structure:

src/
├── components/
│   ├── Nav.tsx           # Navigation bar (handles Login/Logout)
│   ├── Home.tsx          # Simple home page
│   ├── Login.tsx         # Login form
│   ├── TodoList.tsx      # Main container, manages state (CRUD, filters, localStorage)
│   ├── TodoForm.tsx      # Reusable form (Add / Edit)
│   └── TodoItem.tsx      # Individual task display
├── App.tsx               # Main component, manages global state (Auth) and routes
├── index.tsx             # Application entry point
├── index.css             # Global styles (Blue/Green/White palette)
└── setupTests.ts         # Test configuration (for Jest/TypeScript)


💻 Technologies Used
React (with Hooks: useState, useEffect, useMemo)

TypeScript (for strict typing of props and state)

React Router DOM (for navigation)

Native CSS (for styling)

⚙️ Installation and Startup
Follow these steps to run the project locally.

Prerequisites
Node.js and npm/yarn installed.

Steps
Clone the repository (or create the folder):

Bash

git clone [PROJECT_URL]
cd enhanced-todo-list
# If you created the project manually, you are already in the directory.
Install dependencies:

Bash

npm install 
# or 
yarn install
Start the application:

Bash

npm start
# or
yarn start
The application will be accessible in your browser at: http://localhost:3000.