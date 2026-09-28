# 🐍 OOP Wrapper

A simple Python OOP-based Employee Management System that demonstrates important Object-Oriented Programming concepts such as Classes, Objects, Inheritance, Encapsulation, Constructors, Method Overriding, `super()`, Getter/Setter Methods, Destructor, and `issubclass()`.

## 👩‍💻 Student Details

- **Name:** Tanvi Hirapara
- **Project:** OOP Wrapper
- **Language:** Python
- **Tool:** Visual Studio Code

## 🎯 Objective

The objective of this project is to create an Employee Management System using Python Object-Oriented Programming concepts.

The program allows the user to:

- Create a Person
- Create an Employee
- Create a Manager
- Create a Developer
- Display details of created objects
- Check inheritance using `issubclass()`
- Exit the system

## 🧠 OOP Concepts Used

### 1. Class

The project contains different classes:

- `Person`
- `Employee`
- `Manager`
- `Developer`

Each class represents a different type of person or employee.

### 2. Object

Objects are created from the classes to store and display information.

```python
person = Person(name, age)
employee = Employee(name, age, emp_id, salary)
manager = Manager(name, age, emp_id, salary, department)
developer = Developer(name, age, emp_id, salary, language)
```

### 3. Constructor

The `__init__()` method is used as a constructor to initialize object data.

```python
def __init__(self, name, age):
    self.name = name
    self.age = age
```

It automatically runs when an object is created.

### 4. Inheritance

The project uses inheritance between the classes.

```text
Person
   ↓
Employee
   ↓
Manager

Employee
   ↓
Developer
```

- `Employee` inherits from `Person`
- `Manager` inherits from `Employee`
- `Developer` inherits from `Employee`

### 5. Encapsulation

Employee ID and salary are stored as private attributes.

```python
self.__emp_id = emp_id
self.__salary = salary
```

The `__` symbol is used to make these attributes private.

### 6. Getter and Setter

Getter methods are used to access private data.

```python
def get_salary(self):
    return self.__salary
```

Setter methods are used to change private data.

```python
def set_salary(self, salary):
    self.__salary = salary
```

### 7. Method Overriding

The `display()` method is defined in the parent class and redefined in child classes.

```python
def display(self):
    super().display()
    print("Department:", self.department)
```

This is called method overriding.

### 8. super()

The `super()` function is used to call the constructor or method of the parent class.

```python
super().__init__(name, age, emp_id, salary)
```

It allows the child class to use the functionality of its parent class.

### 9. Destructor

The `__del__()` method is used as a destructor.

```python
def __del__(self):
    pass
```

It is related to object destruction and resource cleanup.

### 10. issubclass()

The `issubclass()` function checks whether one class is a child class of another class.

```python
issubclass(Manager, Employee)
issubclass(Developer, Employee)
```

Output:

```text
Manager is subclass of Employee: True
Developer is subclass of Employee: True
```

## ⚙️ Program Features

### 👤 Create Person

The user can enter:

- Name
- Age

Example:

```text
Enter Name: tanvi
Enter Age: 20
```

### 👨‍💼 Create Employee

The user can enter:

- Name
- Age
- Employee ID
- Salary

Example:

```text
Enter Name: aryan
Enter Age: 23
Enter Employee ID: 11
Enter Salary: 80000
```

### 👔 Create Manager

The user can enter:

- Name
- Age
- Employee ID
- Salary
- Department

Example:

```text
Enter Name: bansi
Enter Age: 22
Enter Employee ID: 101
Enter Salary: 60000
Enter Department: sales
```

### 👨‍💻 Create Developer

The user can enter:

- Name
- Age
- Employee ID
- Salary
- Programming Language

Example:

```text
Enter Name: viral
Enter Age: 21
Enter Employee ID: 21
Enter Salary: 60000
Enter Programming Language: python
```

## 📋 Main Menu

The program provides the following menu:

```text
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit
```

## 📊 Show Details

The user can select which object's details they want to display.

```text
Choose details to show:
1. Person
2. Employee
3. Manager
4. Developer
```

If the object has not been created, the program displays:

```text
No Person details available.
```

## 🖥️ Output

```text
--- Python OOP Project: Employee Management System ---

--- Subclass Checking ---
Manager is subclass of Employee: True
Developer is subclass of Employee: True

Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit

Enter your choice: 1
Enter Name: tanvi
Enter Age: 20

Person created with name: tanvi and age: 20

--- Choose another operation ---

Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit

Enter your choice: 2
Enter Name: aryan
Enter Age: 23
Enter Employee ID: 11
Enter Salary: 80000

Employee created with name: aryan age: 23 ID: 11 and salary: $ 80000.0

--- Choose another operation ---

Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit

Enter your choice: 3
Enter Name: bansi
Enter Age: 22
Enter Employee ID: 101
Enter Salary: 60000
Enter Department: sales

Manager created with name: bansi age: 22 ID: 101 salary: $ 60000.0 and department: sales

--- Choose another operation ---

Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit

Enter your choice: 4
Enter Name: viral
Enter Age: 21
Enter Employee ID: 21
Enter Salary: 60000
Enter Programming Language: python

Developer created with name: viral age: 21 ID: 21 salary: $ 60000.0 and programming language: python

--- Choose another operation ---

Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit

Enter your choice: 5

Choose details to show:
1. Person
2. Employee
3. Manager
4. Developer

Enter your choice: 2

Employee Details:
Name: aryan
Age: 23
Employee ID: 11
Salary: $ 80000.0

--- Choose another operation ---

Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit

Enter your choice: 6

Exiting the system. All resources have been freed.
Goodbye!
```

## 📁 Project Structure

```text
OOP_Wrapper/
│
├── OOP_Wrapper.py
└── README.md
```

## 🛠️ Technologies Used

- **Python**
- **Object-Oriented Programming**
- **Visual Studio Code**

## 📌 Project Summary

The **OOP Wrapper** project demonstrates how Python Object-Oriented Programming can be used to create a simple Employee Management System.

The project combines multiple OOP concepts including inheritance, encapsulation, constructor, destructor, method overriding, getter/setter methods, `super()`, and `issubclass()` in one practical program.

## 👩‍💻 Created By

**Tanvi Hirapara**
