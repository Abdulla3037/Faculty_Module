# 🎓 Faculty Management System

This is a **Faculty Management System** which is built using **C**. It keeps all the faculty data in a **Singly Linked List** and lets you add, remove, search, update, and view records all from a straightforward menu right in the terminal.

---

## 📌 What This Project Does

The program gives you a menu when you run it, and you just pick a number to do something. Here's what you can do:

| Option | What it does |
|--------|--------------|
| 0 | Exit the program |
| 1 | Create / Add a new faculty member |
| 2 | Insert a faculty at any position in the list |
| 3 | Delete a faculty from any position |
| 4 | Search for a faculty by their Initial |
| 5 | Modify / Update a faculty's information |
| 6 | Display all faculty members in the list |

---

## 📁 Files in This Project

```
Project/
├── Main.c             → The main file. Runs the menu and handles user input
├── Faculty_Module.c   → All the functions like create, insert, delete, search, etc.
└── Faculty_Module.h   → The header file. Has the struct, enums, and function declarations
```

---

## 🗂️ How the Data is Stored

Each faculty member is stored as a **node** in a linked list. Every node has:

- **Name** : full name of the faculty
- **Initial** : short initials (used for searching)
- **Address** : where they live
- **Phone Number** : contact number
- **Designation** : their academic rank
- **Department** : which department they belong to

### 🏷️ Designations
When entering a designation, use these numbers:

| Number | Designation |
|--------|-------------|
| 1 | Lecturer |
| 2 | Senior Lecturer |
| 3 | Associate Professor |
| 4 | Assistant Professor |
| 5 | Professor |

### 🏫 Departments
When entering a department, use these codes:

| Code | Department |
|------|------------|
| 10 | CSE (Computer Science and Engineering) |
| 11 | EEE (Electrical and Electronic Engineering) |
| 12 | ECE (Electronics and Communication Engineering) |
| 13 | GEB (Genetic Engineering and Biotechnology) |
| 14 | PHARM (Pharmacy) |
| 15 | CE (Civil Engineering) |
| 16 | MPS (Mathematics and Physical Sciences) |
| 20 | English |
| 21 | Law |
| 22 | Social Relations |
| 23 | Information Studies |
| 24 | Sociology |
| 30 | BA (Business Administration) |
| 31 | Economics |

---

## 🛠️ What I Used

- **Singly Linked List** : to dynamically manage the faculty records
- **Dynamic Memory Allocation** : `malloc`, `realloc`, and `free` for handling strings and nodes
- **Enums** : to represent designations and departments cleanly
- **Modular Code** : split into `.h` and `.c` files to keep things organized
- **Input Validation** : so the program doesn't break if you enter a wrong designation or department code

---

## 💡 Some Things Worth Knowing

- The list starts **empty**. So you have to use **Option 1** first before doing anything else like insert, delete, search, etc.
- **Searching** is done by the faculty's **Initial**, not their name. So make sure you remember or note down the initials when adding.
- If you try to insert at a position that's out of range, the program is smart enough to just add the faculty **at the end** instead of crashing.
- When you exit using **Option 0**, all the memory gets properly freed. No memory leaks.
- String input is handled dynamically using `realloc`, so there's no fixed limit on how long a name or address can be.

---

## 🚀 How to Run This Project

> You need **MSYS2 (UCRT64)** and **GCC** installed on your computer.

**Step 1** : Open this file:
```
C:\msys64\ucrt64.exe
```

**Step 2** : Switch to the drive and folder where the project is. For example:
```bash
cd "............../Project"
```
*(Replace the dots with your actual path to the Project folder)*

**Step 3** : Compile and run using this command:
```bash
gcc Main.c Faculty_Module.c -o faculty_module.exe -Wall
./faculty_module.exe
```

That's it! The program should start and show you the menu.

---

## 📋 Using The Menu

Once the program starts, you will see this menu:

```
****Faculty Menu****
0. Exit the programme
1. Create Faculty
2. Insert Faculty At Any Position
3. Delete Faculty At Any Position
4. Search Faculty
5. Modify Faculty
6. Display List for Faculty

Enter your choice:
```

Just type a number and press **Enter** to pick an option. Follow the prompts to enter faculty details.

---

## ⚙️ Requirements

- [MSYS2](https://www.msys2.org/) installed with the UCRT64 environment
- GCC compiler (comes with MSYS2)
- Windows OS

---

## 📝 Project Assumptions

- All inputs (Name, Address, Phone Number) are entered as text strings.
- Designation must be a **positive integer between 1 and 5**.
- Department must be one of the **valid department codes** (10–16, 20–24, 30–31).
- The linked list grows **dynamically** there is no fixed limit on the number of faculty records.
- Memory is properly freed only when you **exit using option 0**.

---

## 🤝 Contributing

If you have any suggestions or want to improve the project, feel free to fork it, make your changes and submit a pull request.

---

## 🔒 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

---

## 📬 Contact

If you have any questions or concerns, please don't hesitate to contact me via email at [abdullahasan220618@gmail.com](mailto:abdullahasan220618@gmail.com)
