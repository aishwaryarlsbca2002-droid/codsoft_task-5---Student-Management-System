# Student Management System

A lightweight Learning Management System (LMS) built with the Django web framework. Designed for schools and colleges to manage students, lecturers, courses, and grading — and a solid project for learning how a full-stack Django app is put together.

## Features

- Admin dashboard with school demographics and analytics
- News and events page, visible to all users
- Admin can add, update, and delete students and lecturers
- Students can add and drop courses
- Lecturers submit scores for attendance, mid-exam, final exam, and assignments
- Automatic calculation of totals, averages, points, and letter grades
- Pass/fail/warning comments generated per student
- Assessment and grade result pages for students, grouped by session and semester
- Course materials: video and document uploads per course
- PDF generation for registration slips and grade reports
- Page-level access restrictions by user role
- Built-in quiz engine:
  - Multiple choice and true/false question types
  - Randomized question order
  - Category-based questions with success-rate tracking
  - Resume incomplete quizzes
  - Configurable pass marks and single-attempt limits
  - Per-question explanations and custom pass/fail messages
  - Marking page for reviewing and grading essay answers

## Requirements

- Python 3.8 or higher

## Getting Started

1. Clone this repository:
```bash
   git clone https://github.com/aishwaryarlsbca2002-droid/Student-Management-System.git
```

2. Create and activate a virtual environment, then install dependencies:
```bash
   pip install -r requirements.txt
```

3. Create a `.env` file in the project root and copy the contents of `.env.example` into it, filling in your own values.

4. Set up the database:
```bash
   python manage.py migrate
```

5. Create an admin account:
```bash
   python manage.py createsuperuser
```

6. Start the development server:
```bash
   python manage.py runserver
```

7. Visit `http://127.0.0.1:8000` in your browser.

## Acknowledgements

- Quiz module adapted from [django_quiz](https://github.com/tomwalker/django_quiz)

## Credits

This project is a locally-run instance of [SkyLearn](https://github.com/SkyCascade/SkyLearn), an open-source LMS created by [Adil Mohak](https://github.com/adilmohak), licensed under MIT.