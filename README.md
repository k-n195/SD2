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

## 3. Scrum Backlog

The following backlog was created using a Scrum-inspired approach to organise and prioritise features required for the system. Each feature was assigned a priority level and included a description and test criteria to ensure it met the project requirements.
<img width="1375" height="621" alt="image" src="https://github.com/user-attachments/assets/45a97854-69f6-4f02-910e-100041ea22cd" />

The following backlog was created using a Scrum-inspired approach to organise and prioritise features required for the system. Each feature was assigned a priority level and included a description and test criteria to ensure it met the project requirements.

## 4. System Design

### 4.1 Overall Architecture
The system was built using a simple client-server structure. The frontend (what the user sees) was created using HTML and CSS, while PHP was used for the backend to handle all the logic and data processing.

Whenever a user performs an action, such as adding or completing a task, the request is sent to the PHP backend. The backend then processes the request and updates the MySQL database. After that, the updated information is retrieved and displayed back to the user.

This approach keeps everything organised by separating the user interface, the logic, and the data. It also makes the system easier to manage and improve in the future.

---

### 4.2 Database Design
The system uses a MySQL database to store all task-related data. The main table used is the "tasks" table, which holds all the information needed for each task.

The table includes the following fields:
- id: A unique ID for each task
- user_id: Links the task to a specific user
- title: The name of the task
- description: Extra details about the task
- due_date: The deadline for the task
- priority: Indicates importance (high, medium, low)
- category: Groups tasks (e.g. work, study, personal)
- status: Shows whether the task is pending or completed
- created_at: Records when the task was created

This structure allows the system to easily store, retrieve, and update tasks. It also supports features like filtering tasks by date and tracking completed tasks.

---

### 4.3 User Interface Design
The user interface was designed to be clean, simple, and easy to use. The aim was to make sure users can quickly understand how to use the system without any confusion.

The main pages in the system include:
- Dashboard: Shows an overview of tasks, including total tasks, completed tasks, and tasks due today
- Tasks Page: Displays all active tasks with options to complete or delete them
- Completed Tasks Page: Shows tasks that have been completed, with options to restore or remove them
- Add Task Page: Allows users to create new tasks
- Calendar: Displays tasks visually based on their due dates, including indicators for days with tasks

A sidebar navigation menu is used across all pages so users can move between sections easily. The design is consistent across the system, which improves usability and makes the overall experience smoother.

Screenshot 1: Dashboard:
<img width="1440" height="810" alt="image" src="https://github.com/user-attachments/assets/a8ee633f-169b-4371-bc4a-8ac9c0dbeecf" />

Screenshot 2- Tasks:
<img width="1440" height="807" alt="image" src="https://github.com/user-attachments/assets/11805ac8-8857-42bb-a8f6-287a511ffbb6" />

Screenshot 3- Completed tasks:
<img width="1440" height="809" alt="image" src="https://github.com/user-attachments/assets/f450ecd4-6202-4db5-8255-d7ba8afa2983" />

Screenshot 4- Add Tasks Form:
<img width="1440" height="810" alt="image" src="https://github.com/user-attachments/assets/9f3c4fe8-6852-4a17-bc9f-233ba2bce411" />

## 5. Implementation
The system was developed using a combination of frontend and backend technologies. HTML and CSS were used to design the layout and overall appearance of the application, focusing on keeping the interface clean and easy to use. PHP was used for the backend to handle all the logic, including processing user input, managing sessions, and communicating with the database. MySQL was used to store all task-related data such as titles, descriptions, due dates, and task status. XAMPP was used as the local development environment, allowing the application to run on a local server during development and testing.

The system includes several key features that were developed step by step throughout the project. Users are able to add new tasks by entering details such as title, description, due date, priority, and category. These tasks are then stored in the database and displayed on the tasks page. Users can view all their active tasks in a structured list, making it easy to see what needs to be done. Tasks can be marked as completed, which moves them to the completed tasks section. If needed, completed tasks can also be restored back to the main task list. The system also allows users to delete tasks permanently, removing them completely from the database.

A mini calendar feature was implemented on the dashboard to give users a visual overview of their tasks. Instead of acting as a full calendar system, it highlights specific dates that contain tasks using small indicators. Users can click on a date to view tasks scheduled for that particular day. This provides a simple but effective way to track tasks without overcomplicating the interface.

Additionally, the dashboard includes a "Due Today" section, which highlights tasks that need to be completed on the current date. A consistent navigation system was implemented using a sidebar, allowing users to move between different pages easily. All features were developed incrementally and tested as they were built, which helped identify and fix issues early.

Below is an example of how a new task is added to the database using PHP:

php:
$sql = "INSERT INTO tasks (user_id, title, description, due_date, priority, category, status)
VALUES ('$user_id', '$title', '$description', '$due_date', '$priority', '$category', '$status')";

This query takes user input from the form and inserts it into the database. Session handling was also implemented to ensure that only logged-in users can access the system:

session_start();
if (!isset($_SESSION['user_id'])) {
    header("Location: login.php");
    exit();
}

## 6. Project Management
The development of this project followed an Agile-inspired approach, where the system was built gradually in stages rather than all at once. Features were implemented step by step, tested, and then improved based on any issues that were identified. This allowed the project to develop in a flexible way and made it easier to fix problems early.

The development process began with planning the layout and structure of the system, including how tasks would be stored and displayed. After this, the basic functionality such as adding and viewing tasks was implemented. Once the core features were working, additional features such as completing tasks, restoring tasks, and deleting tasks were added.

As development progressed, more advanced functionality such as the mini calendar and "Due Today" section were introduced. These features were tested and refined to ensure they worked correctly and improved the overall usability of the system.

Throughout the project, regular testing and adjustments were made. For example, an issue was identified where completed tasks were still showing as active on the calendar. This was resolved by updating the logic to ensure only active tasks were displayed. Other improvements included fixing layout inconsistencies and improving navigation between pages.

A simplified development timeline is shown below:

| Week | Work Completed |
|------|---------------|
| Week 1 | Initial planning, system structure, and UI design |
| Week 2 | Implementing database, login system, and task creation |
| Week 3 | Adding task completion, deletion, restore features, and mini calendar |
| Week 4 | Testing, bug fixes (including calendar issues), and final UI improvements |

This iterative process reflects Agile principles such as continuous improvement, incremental development, and responding to issues as they arise.

7. Tools and Techniques

This project was built using simple and practical tools. Visual Studio Code was used to write and manage the code, and XAMPP was used to run a local server and connect to the database during development and testing.

PHP was used for the backend to handle forms, sessions, and database interaction. MySQL was used to store and manage user and task data. HTML was used to structure the pages, and CSS was used to style the interface and keep it consistent across all pages.

Key techniques included CRUD operations for managing tasks, session handling for secure login, and conditional logic to control features such as task status and calendar indicators.

These tools and techniques were selected as they are appropriate for web-based system development, allowing efficient implementation, testing, and maintenance while meeting both functional and non-functional requirements.

8. Testing and Validation

The system was tested throughout development to ensure it met both user and system requirements. Testing focused on core features such as user login, task creation, task completion, deletion, restoring tasks, and calendar updates.

Each function was tested using normal, boundary, and invalid inputs. For example, task creation was tested with valid inputs, empty fields, and incorrect data formats to ensure proper validation. The login system was tested to confirm that only registered users could access the system using session control.

Special attention was given to the calendar feature, where an issue was identified that completed or deleted tasks were still showing as active (green dots). This was resolved by updating the database query to only display tasks where the status is not completed.

Testing confirmed that all major features work as expected and the system meets its original design requirements. Any issues found during testing were fixed and re-tested to ensure reliability and usability.

PLEASE SEE TEST SD2 WORD DOCUMENT IN REPO FOR TEST TABLE.













