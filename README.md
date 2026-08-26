# 🎬 Cinema Management System
 
A console-based **Cinema Management System** built in **C++** as a 1st semester Programming Fundamentals project. The system allows a cinema administrator to manage **customers/ticket bookings**, **staff records**, and **financial reports** through a simple, menu-driven interface.
 
---
 
## 📖 Overview
 
This project simulates the day-to-day management operations of a cinema, split into three independent modules that are accessed through a central menu after a login screen. It was built to practice core C++ concepts such as structures, arrays, functions, pass-by-reference, and control flow.
 
---
 
## ✨ Features
 
### 🔐 Login System
- Simple username/password authentication before accessing the system.
### 🎟️ Customer Management
- Add a new customer / ticket booking (name, phone, address, ticket type, seat type, showtime)
- Display all booked customers
- Search for a customer by name
- Delete a customer record
- Stores up to 100 customers using a struct array
### 👥 Staff Management
- Add new staff members (ID, name, role, salary)
- Display all staff records
- Update existing staff details by ID
- Delete a staff member by ID
- Stores up to 50 staff members using a struct array
### 💰 Finance Management
- Record total ticket sales
- Record rent, salary, and other expenses
- Automatically calculate total expenses and net profit
- View a complete financial report
- Reset/delete all financial data
### 🎨 Colored Console Output
- Uses the Windows API (`windows.h` / `SetConsoleTextAttribute`) to color-code prompts, success messages, and error messages for a friendlier terminal experience.
---
 
## 🛠️ Technologies Used
 
| Technology | Purpose |
|---|---|
| **C++** | Core programming language |
| **Structures (`struct`)** | Modeling Customer, Staff, and Finance data |
| **Arrays** | Storing customer and staff records |
| **Functions & Pass-by-Reference** | Modular operations on data |
| **`windows.h`** | Console text coloring (Windows-only) |
 
---
 
## 📂 Project Structure
 
```
Cinema_Management_System.cpp   # Single-file source code containing all modules
```
 
The program is organized into three logical modules within `main()`:
1. Customer Management
2. Staff Management
3. Finance Management
Each module runs its own sub-menu loop and returns to the main menu on exit.
 
---
 
## ▶️ How to Run
 
> ⚠️ This program uses `windows.h`, so it must be compiled and run on **Windows** (e.g., using Code::Blocks, Dev-C++, or MSVC/g++ on Windows).
 
**Using g++ (MinGW):**
```bash
g++ Cinema_Management_System.cpp -o CinemaManagementSystem.exe
CinemaManagementSystem.exe
```
 
**Using an IDE:**
1. Open the `.cpp` file in Code::Blocks / Dev-C++ / Visual Studio.
2. Build and Run the project.
**Login credentials (default):**
- Username: *any value*
- Password: `12345`
---
 
## 🖥️ Sample Output
 
Screenshots of the program running are available in the [`screenshots`](./screenshots) folder of this repository.
 
---
 
## 📚 What I Learned
 
- Structuring a multi-module console application in C++
- Working with arrays of structs to manage records
- Passing data between functions by reference for in-place updates
- Implementing basic CRUD (Create, Read, Update, Delete) operations
- Building interactive, menu-driven programs using loops and `switch` statements
---
 
## 🚧 Known Limitations & Future Improvements
 
- Data is stored in memory only and is lost when the program exits (no file/database persistence)
- Fixed-size arrays limit the maximum number of customers (100) and staff (50)
- Login uses a single hardcoded password rather than a secure credential system
- Console coloring restricts portability to Windows; a cross-platform version could use ANSI escape codes instead
- Future versions could add file-based storage (e.g., text files or a database), input validation, and a graphical interface
---
 
## 👤 Author
 
Developed as a 1st Semester Programming Fundamentals project.
 
---
 
## 📄 License
 
This project is open-source and free to use for learning purposes.
 
