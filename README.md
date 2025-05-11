# alu-AirBnB_clone
ALU AirBnB Clone – Command Line Interpreter
 Project Overview
This project is a Command Line Interface (CLI) tool that simulates the backend of an AirBnB-like web application. It allows users to create, retrieve, update, and delete data stored in a persistent file. The project is developed in Python and is part of the foundational curriculum to teach object-oriented programming, data serialization, and command line management.

The project mimics the behavior of a real backend system using object models such as:

BaseModel

User

Place

State

City

Amenity

Review

All interactions are done through a custom console program.

 How to Start
To launch the console in interactive mode, use:

bash
Copy
Edit
$ ./console.py
To run a single command in non-interactive mode, use:

bash
Copy
Edit
$ echo "create User" | ./console.py
How to Use the CLI
Available commands include:

create <class> – Creates a new object of the given class.

show <class> <id> – Displays the string representation of an instance.

destroy <class> <id> – Deletes the specified instance.

all [class] – Prints all instances or all instances of a specified class.

update <class> <id> <attr> <value> – Updates the attribute of an instance.

 Sample Usage
bash
Copy
Edit
(hbnb) create User
1a3b5c7d-8e9f-0123-4567-89abcdef0123

(hbnb) show User 1a3b5c7d-8e9f-0123-4567-89abcdef0123
[User] (1a3b5c7d) {'id': '1a3b5c7d', 'created_at': ..., 'updated_at': ...}

(hbnb) update User 1a3b5c7d name "Victorine"

(hbnb) all User
["[User] (1a3b5c7d) {'id': '1a3b5c7d', 'name': 'Victorine', ...}"]
 Project Structure
bash
Copy
Edit
.
├── console.py              # Entry point of the CLI
├── models/                 # Python classes for all data models
│   ├── base_model.py
│   ├── user.py
│   ├── city.py
│   └── ...
├── models/engine/
│   └── file_storage.py     # Serialization logic (JSON <-> Objects)
├── tests/                  # Unit tests for various components
├── README.md               # Project overview and usage
├── AUTHORS                 # Contributors list
└── .gitignore
 Author
Hikma Hamza
GitHub: Hikma-codes
