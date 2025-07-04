# BUP UCAM Assignment Tracker

A comprehensive assignment management system for Bangladesh University of Professionals (BUP) that eliminates the need for Google Classroom by providing teachers and students with a complete platform to manage assignments, submissions, and grading.

## 🎯 Project Overview

The BUP UCAM Assignment Tracker is designed to streamline assignment management within the university's existing UCAM system. This Object-Oriented Programming (OOP) based solution provides:

- **Teachers**: Create and manage assignments, grade submissions, track student progress
- **Students**: View assignments, submit work, track grades and feedback
- **Administrators**: Oversee the entire system (extensible for future development)

## 🚀 Features

### For Teachers
- ✅ Create and manage courses
- ✅ Create various types of assignments (Homework, Projects, Labs, Quizzes, etc.)
- ✅ Set due dates and maximum marks
- ✅ View and grade student submissions
- ✅ Provide detailed feedback
- ✅ Track assignment statistics and student participation
- ✅ Monitor late submissions

### For Students
- ✅ View enrolled courses and available assignments
- ✅ Submit assignments with text content
- ✅ Track submission status and deadlines
- ✅ View grades and teacher feedback
- ✅ Monitor overall academic performance

### System Features
- ✅ User authentication and role-based access
- ✅ Real-time assignment status tracking
- ✅ Comprehensive reporting and statistics
- ✅ Late submission detection
- ✅ Grade calculation and performance analytics

## 🏗️ Architecture

The system follows Object-Oriented Programming principles with a clear separation of concerns:

```
src/main/java/org/app/
├── model/           # Core data models
│   ├── User.java           # Abstract base user class
│   ├── Teacher.java        # Teacher-specific functionality
│   ├── Student.java        # Student-specific functionality
│   ├── Course.java         # Course management
│   ├── Assignment.java     # Assignment entities
│   ├── Submission.java     # Student submissions
│   └── Enums/             # Status and type definitions
├── service/         # Business logic layer
│   ├── UserService.java        # User management operations
│   ├── CourseService.java      # Course operations
│   └── AssignmentService.java  # Assignment and submission logic
└── controller/      # Application interface
    └── AssignmentTrackerController.java  # Main application controller
```

## 🛠️ Technology Stack

- **Language**: Java 23
- **Build Tool**: Maven
- **Dependencies**:
  - Jackson (JSON processing)
  - Java Time API (Date/Time handling)
- **Architecture**: MVC Pattern with Service Layer

## 📋 Prerequisites

- Java 23 or higher
- Maven 3.6+
- IDE (IntelliJ IDEA recommended)

## 🚦 Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd "Assignment Tracker Final"
   ```

2. **Build the project**
   ```bash
   mvn clean compile
   ```

3. **Run the application**
   ```bash
   mvn exec:java -Dexec.mainClass="org.app.Main"
   ```

## 👥 Sample Data

The system comes pre-loaded with sample data for testing:

### Teachers
- **Dr. Ahmed Rahman** (Computer Science)
  - Email: ahmed@bup.edu.bd
  - Password: password123

- **Prof. Sarah Khan** (Business Administration)
  - Email: sarah@bup.edu.bd
  - Password: password123

### Students
- **Mohammad Ali** (CSE, Semester 7)
  - Email: ali@student.bup.edu.bd
  - Password: student123

- **Fatima Hassan** (CSE, Semester 7)
  - Email: fatima@student.bup.edu.bd
  - Password: student123

### Courses
- Object Oriented Programming (CSE-202)
- Business Management (BBA-101)

## 🎮 Usage Guide

### For Teachers

1. **Login** with teacher credentials
2. **Create Course**: Set up new courses with details
3. **Create Assignment**: 
   - Select course and assignment type
   - Set title, description, and due date
   - Define maximum marks
4. **Grade Submissions**: Review student work and provide feedback
5. **View Statistics**: Monitor course and assignment performance

### For Students

1. **Login** with student credentials
2. **View Assignments**: See all available assignments across courses
3. **Submit Work**: Submit assignments before due dates
4. **Track Progress**: Monitor submission status and grades
5. **View Feedback**: Read teacher comments and improve

## 🔧 Key Classes and Methods

### Core Models
- `User` (Abstract): Base class for all users
- `Teacher`: Extends User, manages courses and assignments
- `Student`: Extends User, handles submissions and enrollment
- `Assignment`: Represents assignments with due dates and grading
- `Submission`: Student work submissions with grading capability

### Services
- `UserService`: Authentication and user management
- `CourseService`: Course creation and enrollment
- `AssignmentService`: Assignment lifecycle and grading

## 📊 Assignment Types Supported

- Homework
- Project
- Lab Assignment
- Quiz
- Exam
- Presentation
- Research Paper
- Case Study

## 🔄 Assignment Status Flow

1. **Draft** → **Active** → **Closed** → **Graded** → **Archived**

## 📈 Future Enhancements

- File attachment support for assignments and submissions
- Email notifications for due dates and grading
- Advanced reporting and analytics
- Mobile application interface
- Integration with existing BUP systems
- Plagiarism detection
- Bulk operations for teachers
- Parent/Guardian access portal

## 🤝 Contributing

This project is developed for Bangladesh University of Professionals. For contributions:

1. Fork the repository
2. Create a feature branch
3. Make your changes following OOP principles
4. Test thoroughly
5. Submit a pull request

## 📝 License

This project is developed for educational purposes as part of the BUP UCAM system enhancement initiative.

## 📞 Support

For technical support or feature requests, please contact the BUP IT Department.

---

**Developed with ❤️ for Bangladesh University of Professionals**

*Making assignment management efficient and effective for the BUP community.*
