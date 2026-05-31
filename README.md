# 🎓 School Result Management System (SQL Project)

## 📌 Project Overview

Created a relational database system built using MySQL to simulate a real-world school result management platform.

The database manages:

* Student records
* Subject allocation
* Student subject registration
* Test and examination scores
* Total score computation
* Student performance analysis

The system demonstrates practical SQL concepts including:

* Relational database design
* Query automation
* Data modeling
* SQL joins
* Result analytics

---

# 🧱 Database Structure

The project contains four major tables:

## 1. `students`

Stores student information.

| Column       | Description       |
| ------------ | ----------------- |
| student_id   | Unique student ID |
| student_name | Student full name |
| gender       | Student gender    |
| class_name   | Student class     |

---

## 2. `subjects`

Stores all school subjects.

| Column       | Description       |
| ------------ | ----------------- |
| subject_id   | Unique subject ID |
| subject_name | Subject name      |

---

## 3. `student_subjects`

Maps students to registered subjects.

| Column     | Description |
| ---------- | ----------- |
| id         | Record ID   |
| student_id | Student ID  |
| subject_id | Subject ID  |

---

## 4. `results`

Stores student performance records.

| Column      | Description        |
| ----------- | ------------------ |
| score_id    | Result ID          |
| student_id  | Student ID         |
| subject_id  | Subject ID         |
| test_score  | Test score (/40)   |
| exam_score  | Exam score (/60)   |
| total_score | Total score (/100) |

---
## 🧱 Database Tables

![Tables](https://github.com/Oghenefegor-Annabel/school-result-management-sql/blob/main/Screenshot%202026-05-29%20170450.png?raw=true)

# ⚙️ Features

* Automated result generation
* Subject assignment system
* Random score simulation
* Test and exam score computation
* Relational database normalization
* Student performance tracking
* Analytics-ready dataset

---

# 🧠 SQL Concepts Used

This project demonstrates the use of:

* CREATE TABLE
* INSERT INTO
* INNER JOIN
* FOREIGN KEY relationships
* Aggregate Functions
* CASE Statements
* GROUP BY
* Automated SQL queries
* Random data generation using `RAND()`

---

# 📊 Sample Automated SQL Query

```sql
INSERT INTO results (
    student_id,
    subject_id,
    test_score,
    exam_score,
    total_score
)

SELECT
    ss.student_id,
    ss.subject_id,

    FLOOR(RAND() * 41) AS test_score,
    FLOOR(RAND() * 61) AS exam_score,

    FLOOR(RAND() * 41) + FLOOR(RAND() * 61) AS total_score

FROM student_subjects ss;
```

---

# 📈 Sample Analysis

The database can be used to analyze:

* Top-performing students
* Average subject performance
* Pass/fail rates
* Class performance comparison
* Student ranking
* Subject trends

---

# 🖥 Tools Used

* MySQL
* MySQL Workbench
---

# 🚀 Future Improvements

Potential upgrades include:

* Attendance management system
* Teacher management module
* GPA calculation
* Report card generation
* Web application integration
* Student portal dashboard

---

# 📚 What I Learned

Through this project, I improved my understanding of:

* Relational database design
* SQL automation
* Data modeling
* Query optimization
* Educational data analysis
* Database relationships

---

# 👨‍💻 Author

OGBE OGHENEFEGOR ANNABEL

Data Analyst
