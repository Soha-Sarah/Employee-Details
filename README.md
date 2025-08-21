This project demonstrates Object-Oriented Programming (OOP) concepts in Python using an Employee class hierarchy.  
It models different employee types like Managers and Developers, showcasing inheritance, encapsulation, and method overriding.  

# Features  

- Base Employee class with common attributes (name, ID, salary)  
- Annual salary calculation based on monthly salary  
- Manager subclass with department management and leave approval  
- Developer subclass with programming language specialization and code-writing behavior  

## Demonstrates OOP concepts:  

- Encapsulation  
- Inheritance  
- Method overriding  

# Classes  

### Employee (Base Class)  

#### Attributes:  

- Name  
- ID  
- Salary  
- AnnualSalary (calculated)  

#### Methods:  

- Display() → prints name, ID, and salary  
-AnnualSalary() → prints annual salary  

### Manager (Subclass of Employee)  

#### Attributes:  

- Department  

#### Methods:  

- Display() → prints employee details + department  

- ApproveLeave(EmployeeName) → approves leave for employees   

### Developer (Subclass of Employee)  

#### Attributes:  

- ProgrammingLanguage  

#### Methods:  

- Display() → prints employee details + programming language
- WriteCode() → simulates writing code

# Example Usage:  
```python
# Create Employees
e1 = Employee("Alice", 101, 3000)
m1 = Manager("Bob", 102, 5000, "IT")
d1 = Developer("Charlie", 103, 4000, "Python")

# Display Employee Info
e1.Display()
e1.AnnualSalary()

# Manager Info
m1.Display()
m1.ApproveLeave("Alice")

# Developer Info
d1.Display()
d1.WriteCode()
```
# Output:  
```python
Name:  Alice
ID Number:  101
Salary:  3000
Annual Salary:  36000

Name:  Bob
ID Number:  102
Salary:  5000
Department:  IT
Leave approved for: Alice

Name:  Charlie
ID Number:  103
Salary:  4000
The programming language used:  Python
Writing code in:  Python
```
