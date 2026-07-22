# Student-Management-System
# Student Management System

A lightweight, menu-driven **Student Management System** built in Python. Every
record is stored directly in a plain text file — no external database
required — making the project easy to run, read, and extend.

## Features

- **Add Student** — create a new record with validated ID, name, age, course, and marks
- **Display Students** — list every record currently stored
- **Search Student** — look up a single record by Student ID
- **Update Student** — edit an existing student's details
- **Delete Student** — remove a record by ID
- **Average Marks** — class average, computed with NumPy
- **Highest Marks** — student(s) with the top score
- **Lowest Marks** — student(s) with the lowest score

## Tech Stack

| Component | Choice |
|---|---|
| Language | Python 3 |
| Storage | Plain text file (`students.txt`) |
| Interface | Command-line menu |
| Numeric ops | NumPy |

## Data Format

Each line in `students.txt` represents one student as comma-separated values:

\```
id,name,age,course,marks
\```

Example:

\```
21,arsal,21,english,90.0
1,ali,20,english,70.0
\```

## Getting Started

### Prerequisites

- Python 3.8+
- NumPy (`pip install -r requirements.txt`)

### Run

\```bash
python student_management.py
\```

You'll see a numbered menu with options to add, display, search, update, delete, and analyze records.

## Project Structure

\```
.
├── student_management.py
├── notebooks/student_management_system.ipynb
├── data/students_sample.txt
├── requirements.txt
└── README.md
\```

## Input Validation

| Field | Rule |
|---|---|
| Student ID | Digits only |
| Name | Alphabetic characters only |
| Age | Positive integer |
| Course | Alphabetic characters only |
| Marks | Numeric, between 0 and 100 |

## Future Enhancements

- Migrate storage to SQLite or another database
- Add a graphical (GUI) or web-based interface
- Support CSV export and bulk record import
- Add authentication for admin-only access

## License

MIT License
