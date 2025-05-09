# 🎓 MySQL Student Management System

A Python 3.13-based desktop application designed to manage student records efficiently using MySQL. This project demonstrates CRUD (Create, Read, Update, Delete) operations with a user-friendly interface, making it ideal for educational institutions and administrative tasks.

---

## 📖 Table of Contents

- [🎓 MySQL Student Management System](#-mysql-student-management-system)
- [📖 Table of Contents](#-table-of-contents)
- [🧑‍💼 User Experience (UX)](#-user-experience-ux)
  - [🧾 User Stories](#-user-stories)
- [🎨 Design](#-design)
  - [🗂 Interface Structure](#-interface-structure)
  - [🌈 Color Scheme & Typography](#-color-scheme--typography)
- [🚀 Features](#-features)
  - [✅ Implemented Features](#-implemented-features)
  - [🛠️ Planned Improvements](#-planned-improvements)
- [💻 Technologies Used](#-technologies-used)
  - [🧑‍💻 Languages Used](#-languages-used)
  - [📚 Libraries Used](#-libraries-used)
- [📁 Project Files](#-project-files)
- [🛠 Installation & Usage](#-installation--usage)
  - [⚙️ How to Run](#-how-to-run)
  - [🧾 Database Configuration](#-database-configuration)
- [✅ Testing](#-testing)
- [🙌 Credits](#-credits)
  - [👨‍💻 Author](#-author)
  - [🧰 Tools & Technologies](#-tools--technologies)
  - [📚 Learning Resources & Documentation](#-learning-resources--documentation)
  - [💡 Inspiration](#-inspiration)
  - [🤝 Contributions](#-contributions)

---

## 🧑‍💼 User Experience (UX)

### 🧾 User Stories

**As an administrator**, I want to:

- Add new student records with details like name, age, and course.
- View a list of all students in the database.
- Update existing student information.
- Delete student records when necessary.

**As a user**, I want to:

- Search for a student by name or ID.
- Navigate the application with ease and clarity.

---

## 🎨 Design

### 🗂 Interface Structure

The application features a graphical user interface (GUI) built with Tkinter, comprising:

- **Input Fields**: For entering student details.
- **Buttons**: To execute actions like Add, Update, Delete, and Search.
- **Display Area**: A table or listbox showing current student records.

### 🌈 Color Scheme & Typography

- **Color Scheme**: Neutral tones for a professional appearance.
- **Typography**: Standard system fonts for readability.

---

## 🚀 Features

### ✅ Implemented Features

- **Add Student**: Input and save new student details to the MySQL database.
- **View Students**: Display all student records in a structured format.
- **Update Student**: Modify existing student information.
- **Delete Student**: Remove student records from the database.
- **Search Functionality**: Find students by name or ID.
- **Data Persistence**: All data is stored in a MySQL database.

### 🛠️ Planned Improvements

- **Input Validation**: Ensure all fields are correctly filled before submission.
- **Enhanced Search**: Implement advanced search filters (e.g., by course or age).
- **User Authentication**: Add login functionality for administrators.
- **Export Data**: Allow exporting student records to CSV or PDF formats.
- **Responsive Design**: Improve GUI layout for different screen sizes.

---

## 💻 Technologies Used

### 🧑‍💻 Languages Used

- Python 3.13

### 📚 Libraries Used

- `tkinter`: For building the GUI.
- `mysql-connector-python`: For connecting to the MySQL database.

---

## 📁 Project Files

```bash
mysql-student-management-system/
├── main.py # Main application script
├── requirements.txt # List of dependencies
├── README.md # Project documentation
└── icons/ # Folder containing icon images
```

---

## 🛠 Installation & Usage

### ⚙️ How to Run

1. **Clone the repository**:

   ```bash
   git clone https://github.com/mahmudurmahid/mysql-student-management-system.git
   cd mysql-student-management-system
   ```

2. Install dependencies:

Ensure you have Python 3.13 installed. Install required libraries:

```bash
pip install -r requirements.txt
```

3. Run the application:

```bash
python main.py
```

### 🧾 Database Configuration

1. Install MySQL Server:

Download and install MySQL Server from the official website.

2. Create a Database:

Log in to your MySQL server and create a new database:

```bash
CREATE DATABASE student_management;
```

3. Create a Table:

Use the following SQL script to create the students table:

```bash
USE student_management;

CREATE TABLE students (
id INT AUTO_INCREMENT PRIMARY KEY,
name VARCHAR(100) NOT NULL,
age INT NOT NULL,
course VARCHAR(100) NOT NULL
);
```

4. Update Database Credentials:

In the main.py file, update the database connection parameters with your MySQL credentials:

```bash
db = mysql.connector.connect(
host="localhost",
user="your_username",
password="your_password",
database="student_management"
)
```

## ✅ Testing

Manual testing has been conducted to ensure:

- Accurate addition of new student records.
- Proper display of all student data.
- Successful updating and deletion of records.
- Effective search functionality.

### 🙌 Credits

#### 👨‍💻 Author

- **Mahmudur Mahid**
  - GitHub: [@mahmudurmahid](https://github.com/mahmudurmahid)
  - Python Developer and Computer Science Enthusiast with a focus on building real-world, problem-solving applications for education and productivity.

#### 🧰 Tools & Technologies

- **Python 3.13**  
  The core programming language used to develop the backend logic of the application.
- **MySQL Server**  
  An open-source relational database used to store and manage student data efficiently.
- **MySQL Connector for Python**  
  A library used to connect Python to MySQL, enabling smooth communication between the application and the database.
- **Tkinter**  
  Python’s built-in GUI library used to create a clean and simple desktop interface for user interaction.
- **DB Browser for SQLite** (used in related projects)  
  Though not used in this exact project, it served as inspiration for database schema design and debugging workflows.

#### 📚 Learning Resources & Documentation

- [Python Official Documentation](https://docs.python.org/3/)
- [MySQL Connector Python Documentation](https://dev.mysql.com/doc/connector-python/en/)
- [Real Python](https://realpython.com/)
  - For in-depth tutorials on Tkinter GUI development and MySQL integration.
- [Stack Overflow](https://stackoverflow.com/)
  - For solving issues related to database connections, Tkinter widget behaviors, and error handling.
- [GeeksforGeeks Python Tutorials](https://www.geeksforgeeks.org/python-programming-language/)
  - Provided guidance and examples on CRUD operations and GUI layout management.

#### 💡 Inspiration

- Inspired by traditional student management systems used in educational institutions.
- Driven by the desire to learn more about Python GUIs and database integration in a real-world scenario.

#### 🤝 Contributions

- This project is currently authored and maintained by a single developer.
- Contributions in the form of bug fixes, feature suggestions, testing feedback, and enhancements are welcome.

  If you'd like to contribute:

  1. Fork the repository.
  2. Create a feature branch.
  3. Submit a pull request with a clear description of changes.
