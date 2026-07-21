# Student Record & Grade Management System (CLI)

**Intern Name:** [Husnain Shoukat]
**Intern Batch:** [2026]
**Track:** Week 1 — Python Fundamentals + Mini Project
**Company:** OvacSol Pvt. Ltd.

A command-line application to add, update, view, and delete student
records, with automatic total/average/grade calculation and persistent
storage in JSON.

## Project Structure

```
student_project/
├── main.py            # Menu loop / entry point
├── student.py          # Student class (OOP)
├── file_manager.py     # Save/load logic (JSON + CSV)
├── students.json        # Sample data file (auto-created/updated)
├── requirements.txt
└── README.md
```

## Setup Instructions

### 1. Create a virtual environment

```bash
python -m venv venv
```

### 2. Activate it

**Windows:**
```bash
venv\Scripts\activate
```

**Mac/Linux:**
```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the program

```bash
python main.py
```

## Usage

You'll see a menu with 6 options:

```
1. Add Student
2. Update Marks
3. View Single Student
4. View All Students
5. Delete Student
6. Save & Exit
```

- Records are kept in memory while the program runs and written to
  `students.json` when you choose **Save & Exit**.
- On the next run, the program automatically reloads `students.json`,
  so your data survives between sessions.

## Notes

- If `tabulate` isn't installed, the program still works — it falls
  back to a plain-text table for "View All Students".
- Invalid input (non-numeric marks, out-of-range marks, missing
  students, corrupted data files) is caught and reported without
  crashing the program.
"# Student-Record-Management-System" 
