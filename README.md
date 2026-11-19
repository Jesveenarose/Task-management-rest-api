# Task Management REST API

A secure, user-isolated backend RESTful API built with *Python, **Django, and **Django REST Framework (DRF)* that allows registered users to create, read, update, and delete daily tasks.

## Tech Stack
* *Language:* Python 3
* *Framework:* Django, Django REST Framework (DRF)
* *Database:* SQLite3 (Django ORM)
* *Authentication:* Session & Permission-based (IsAuthenticated)

## Key Features
* *User Registration:* New users can register securely with password hashing.
* *Task CRUD Operations:* Full Create, Read, Update, and Delete support for tasks.
* *Data Isolation:* Users can only view and manage their own tasks via queryset filtering.
* *Status Tracking:* Supports PENDING, IN_PROGRESS, and COMPLETED task states along with due dates.

## API Endpoints
| Method | Endpoint | Description | Access |
| :--- | :--- | :--- | :--- |
| POST | /api/register/ | Register a new user account | Public |
| GET | /api/tasks/ | Retrieve all tasks for logged-in user | Authenticated |
| POST | /api/tasks/ | Create a new task | Authenticated |
| PUT | /api/tasks/<id>/ | Update an existing task | Authenticated |
| DELETE | /api/tasks/<id>/ | Delete a task | Authenticated |

## How to Run Locally
1. Clone the repository:
   ```bash
   git clone [https://github.com/Jesveenarose/Task-management-rest-api.git](https://github.com/Jesveenarose/Task-management-rest-api.git)
   cd Task-management-rest-api
