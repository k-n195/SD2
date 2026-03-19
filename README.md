# Personal Task Planner.

## 1. Introduction
This project involves the design and development of a Personal Task Planner web application. The purpose of the system is to help users organise, manage, and track their daily tasks in an efficient and user-friendly way. The application allows users to create tasks, assign priorities, set due dates, and monitor their progress through a structured interface.
The system was developed to address common issues with task management such as lack of organisation, missed deadlines, and difficulty tracking completed work. By providing a clear dashboard, task lists, and a calendar view, the application improves productivity and helps users stay on top of their responsibilities.
The target users for this system include students and individuals who need a simple and effective way to manage their workload. The design focuses on usability, simplicity, and accessibility, ensuring that users can quickly interact with the system without requiring advanced technical knowledge.
Key features of the system include task creation, editing, deletion, completion tracking, and a calendar that visually highlights upcoming tasks. The system also includes user authentication to ensure that each user can securely manage their own tasks.
Overall, this project demonstrates the development of a full-stack web application using PHP, MySQL, HTML, and CSS, combining both frontend design and backend functionality to deliver a complete working system.

## 2. User and System Requirements
### 2.1 User Requirements
The following user requirements were identified for the system. These describe what the end user should be able to do when interacting with the application.
- The user should be able to create new tasks with a title, description, due date, priority, and category.
- The user should be able to view all tasks in a structured list.
- The user should be able to mark tasks as completed.
- The user should be able to restore completed tasks if needed.
- The user should be able to delete tasks permanently.
- The user should be able to view tasks filtered by specific dates using a calendar interface.
- The user should be able to view tasks due on the current day.
- The user should be able to navigate easily between dashboard, tasks, and completed tasks pages.
- The user should be able to securely log in and access their own tasks only.
These requirements were prioritised based on their importance to the core functionality of the system. Task creation, viewing, and completion were considered high priority, as they are essential to the usability of the application.

### 2.2 System Requirements
The system requirements define the technical and functional components needed to support the user requirements.
- The system must use a MySQL database to store user and task data.
- The system must implement CRUD functionality (Create, Read, Update, Delete) for tasks.
- The system must use PHP for backend processing and server-side logic.
- The system must use HTML and CSS to provide a responsive and user-friendly interface.
- The system must implement session management to securely handle user authentication.
- The system must ensure that each user can only access their own data.
- The system must dynamically update task status (e.g. pending, completed).
- The system must visually display tasks on a calendar using indicators.
- The system must update the calendar dynamically when tasks are completed or deleted.
- The system must provide smooth navigation between all pages.
These requirements ensure that the system is functional, secure, and capable of handling user interactions effectively.

### 2.3 Scrum User Stories
An Agile-inspired approach was used during development, where features were built incrementally and improved through continuous testing and feedback. Scrum-style user stories were used to define the system from the user’s perspective and guide development decisions.
- As a user, I want to create a task so that I can keep track of my work.
- As a user, I want to assign a due date to tasks so that I can meet deadlines.
- As a user, I want to set task priorities so that I can focus on important tasks first.
- As a user, I want to mark tasks as completed so that I can track my progress.
- As a user, I want to delete tasks so that I can remove unnecessary items.
- As a user, I want to restore completed tasks so that I can reuse them if needed.
- As a user, I want to view tasks for a specific day so that I can plan my schedule.
- As a user, I want to see tasks displayed on a calendar so that I have a visual overview.
- As a user, I want to log in securely so that my data is protected.
- As a user, I want an easy-to-use interface so that I can manage tasks efficiently.
These user stories supported an iterative development process, where features were gradually implemented, tested, and refined. This reflects Agile principles such as continuous improvement, user-focused design, and incremental delivery.
