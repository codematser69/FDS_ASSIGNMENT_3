# FDS_ASSIGNMENT_3
# TaskFlow - To-Do Web Application

## 1. Project Overview

TaskFlow is a web-based To-Do application developed using the Django framework and Python. The purpose of this project is to provide a simple interface for creating and viewing tasks while demonstrating the fundamental concepts of Django web development.

The application uses Django's Model-View-Template (MVT) architecture and SQLite as the database. Users can add tasks through the web interface, and the tasks are stored persistently in the database.

---

## 2. Objectives

The main objectives of this project are:

- To understand the fundamentals of the Django framework.
- To implement a basic web application using Python and Django.
- To understand Django's Model-View-Template architecture.
- To create and manage database records using Django models.
- To handle HTML forms and HTTP requests.
- To understand URL routing in Django.
- To develop a clean and responsive web interface.
- To understand the use of Django's built-in administration system.

---

## 3. Features

The application provides the following features:

- Add new tasks.
- Display all stored tasks.
- Store tasks in a SQLite database.
- Display the date on which each task was created.
- Indicate completed tasks using a checkbox.
- Provide a clean and responsive user interface.
- Manage task records through the Django Admin panel.

---

## 4. Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Backend programming language |
| Django | Web application framework |
| HTML | Structure of the web pages |
| CSS | Styling and responsive design |
| SQLite | Database management |
| Git | Version control |
| GitHub | Source code hosting |

---

## 5. Project Architecture

This project follows Django's Model-View-Template (MVT) architecture.

### Model

The `Task` model defines the structure of task data stored in the database.

The model contains:

- `title` - Stores the task name.
- `completed` - Stores the completion status of the task.
- `created_at` - Stores the date and time when the task was created.

### View

The view handles requests from the user, retrieves tasks from the database, processes submitted forms, creates new tasks, and sends data to the template.

### Template

The HTML template is responsible for displaying the user interface and the tasks retrieved from the database.

### URL Configuration

Django URL configurations connect incoming web requests to the appropriate view functions.

---

## 6. Project Structure

```text
django_project/
│
├── manage.py
├── db.sqlite3
├── README.md
│
├── todo_project/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
└── tasks/
    ├── migrations/
    │   ├── __init__.py
    │   └── 0001_initial.py
    │
    ├── templates/
    │   └── tasks/
    │       └── task_list.html
    │
    ├── __init__.py
    ├── admin.py
    ├── apps.py
    ├── models.py
    ├── tests.py
    ├── urls.py
    └── views.py
