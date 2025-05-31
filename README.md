# Task Master (TodoList)

A simple, clean, and lightweight Flask-based To-Do List web application that allows you to:

- Create new tasks
- View all tasks in an organized table
- Update existing tasks
- Delete tasks

Tasks are stored in a SQLite database via SQLAlchemy, and the UI is rendered using Jinja2 templates. The app is styled with a modern, responsive CSS design.

---

## Table of Contents

1. [Features](#features)  
2. [Demo Screenshot](#demo-screenshot)  
3. [Tech Stack](#tech-stack)  
4. [Folder Structure](#folder-structure)  
5. [Installation](#installation)  
6. [Usage](#usage)  
7. [Database Model](#database-model)  
8. [Routes & Templates](#routes--templates)  
9. [Customizing CSS](#customizing-css)  
10. [Contributing](#contributing)  
11. [License](#license)  

---

## Features

- **Add Tasks**  
  Users can enter a new task via a simple form. Each task is timestamped with the creation date.
- **View Tasks**  
  All tasks are displayed in a striped, hover-highlighted HTML table. If no tasks exist, a placeholder message is shown.
- **Update Tasks**  
  Each row has an “Update” link. Clicking it opens a form pre-filled with the existing task content, allowing you to modify it.
- **Delete Tasks**  
  Each row has a “Delete” link. Clicking it removes the task from the database immediately.
- **SQLite + SQLAlchemy**  
  Tasks are persisted in a local SQLite file (`test.db`) using SQLAlchemy ORM.
- **Responsive Design**  
  The CSS is fully responsive: desktop tables collapse into mobile-friendly card layouts on narrow viewports.

---

## Demo Screenshot

> _Note: You can replace this placeholder with an actual screenshot once you run the app._

![Task Master Screenshot](./static/todo_screenshot.png)  
_(Example: index page showing several tasks with Update/Delete links.)_

---

## Tech Stack

- **Framework**: Flask (Python)  
- **Database**: SQLite (via Flask-SQLAlchemy)  
- **Templating**: Jinja2  
- **Styling**: Custom responsive CSS  
- **Python Version**: 3.7+  

---

## Folder Structure

TodoList/
├── app.py
├── requirements.txt
├── test.db # created after first run
├── README.md
├── static/
│ └── style.css # main stylesheet for “ultra-fancy” design
│
└── templates/
├── base.html # base template: common HTML head + CSS link
├── index.html # main page: list tasks + add new
├── update.html # form to edit an existing task
└── 404.html # optional: custom 404 page (if added)


TodoList/
├── app.py
├── requirements.txt
├── test.db # created after first run
├── README.md
├── static/
│ └── style.css # main stylesheet for “ultra-fancy” design
│
└── templates/
├── base.html # base template: common HTML head + CSS link
├── index.html # main page: list tasks + add new
├── update.html # form to edit an existing task
└── 404.html # optional: custom 404 page (if added)
