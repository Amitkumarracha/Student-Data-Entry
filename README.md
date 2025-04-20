
---

```markdown
# 📚 Student Management System with Exception Handling  
-- Directly Committed from GIT BASH --

## 📖 Project Description  
This Java-based Student Management System demonstrates the use of **Object-Oriented Programming (OOP)** and **Custom Exception Handling**. The project allows the user to add, view, search, update, and delete student records from a list.

Each functionality is split into separate, well-structured classes. The application also uses multiple **user-defined exceptions** to provide robust error handling, ensuring a smooth and intuitive experience for the user.

---

## 📂 Project Structure  

```
StudentManagement/
│── Main.java                        # Main class with the user menu  
│── Operations.java                  # Contains all student-related operations  
│── Student.java                     # Data model class for student details  
│── CustomException.java             # Parent class for all custom exceptions  
│── DuplicateStudentException.java   # Thrown when a duplicate PRN is detected  
│── InvalidChoiceException.java      # Thrown when an invalid menu option is entered  
│── InvalidInputException.java       # Thrown for invalid user input formats  
│── StudentNotFoundException.java    # Thrown when a student is not found in the list  
│── (Optional: .class files)         # Compiled bytecode (generated after compiling)
```

---

## ⚡ Functions & Features  

| 📄 File Name               | 🔧 Method / Class Name          | 📌 Description |
|---------------------------|----------------------------------|----------------|
| `Main.java`               | `main()`                         | Entry point; displays menu and handles user choices |
| `Operations.java`         | `addStudent()`                   | Adds a new student to the list with duplicate check |
|                           | `displayAllStudents()`           | Shows all student records |
|                           | `searchStudentByPRN()`           | Search using PRN |
|                           | `searchStudentByName()`          | Search using name |
|                           | `searchStudentByPosition()`      | Search using list position |
|                           | `updateStudent()`                | Modify existing student details |
|                           | `deleteStudent()`                | Remove a student by PRN |
| `Student.java`            | `Student` class                  | Defines attributes: PRN, name, DOB, marks |
| `CustomException.java`    | Superclass                       | Parent class for all custom exceptions |
| `DuplicateStudentException.java` | Exception class         | Raised when adding a student with existing PRN |
| `StudentNotFoundException.java` | Exception class         | Raised when search/delete fails due to invalid PRN |
| `InvalidInputException.java` | Exception class              | Raised for invalid inputs (e.g., wrong format) |
| `InvalidChoiceException.java` | Exception class             | Raised when an invalid menu choice is entered |

---

## 🧠 Exception Handling  

This project uses a combination of **custom** and **built-in** exceptions to handle all possible user and system errors effectively:

### ✅ List of Custom Exceptions:
- `DuplicateStudentException` — Prevents adding a student with duplicate PRN  
- `InvalidInputException` — Validates user inputs like numbers and formats  
- `InvalidChoiceException` — Catches menu selections outside valid range  
- `StudentNotFoundException` — Triggers when no student found for PRN/position

All exception classes inherit from `CustomException`, making the code scalable and modular.

---

## 🛠️ How to Compile & Run

1. **Open Terminal / Git Bash**
2. **Navigate to your project folder**:
   ```bash
   cd path/to/StudentManagement
   ```
3. **Compile all Java files**:
   ```bash
   javac *.java
   ```
4. **Run the program**:
   ```bash
   java Main
   ```

---

## 🧪 Input Example

```text
Enter PRN: 2300456789  
Enter Name: Raj Sharma  
Enter DOB: 2002-04-17  
Enter Marks: 89.5  
```

---

## ✅ Highlights

- ✨ Clean modular design  
- 🚫 No hardcoded values  
- 🔁 Continuous input until Exit  
- 📢 User-friendly error messages  
- ✅ All operations tested with both valid and invalid inputs  

---

## 🔍 Final Notes

- Designed using Java SE (Standard Edition)
- Console-based menu system
- Tested in Windows 10 using Git Bash and Command Prompt
- Easy to extend: You can add file-based storage or GUI later

---

## 📝 Developer Info

- 👨‍💻 **Name**: Amitkumar Racha

---

```