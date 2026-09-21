# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
```python
class Details:
    def getName(self):
        self.name = input("Enter name: ")
    def getAge(self):
        self.age = int(input("Enter age: "))
class Employee(Details):
    def getEmployeeDetails(self):
        self.employee_id = input("Enter employee ID: ")
        self.department = input("Enter department: ")
        print("Employee Name:", self.name)
        print("Employee Age:", self.age)
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)
class Patient(Details):
    def getPatientDetails(self):
        self.patient_id = input("Enter patient ID: ")
        self.disease = input("Enter disease: ")
        print("Patient Name:", self.name)
        print("Patient Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)
e = Employee()
e.getName()
e.getAge()
e.getEmployeeDetails()
p = Patient()
p.getName()
p.getAge()
p.getPatientDetails()
```
## Sample Output

<img width="773" height="530" alt="image" src="https://github.com/user-attachments/assets/9d434fff-c4de-47dd-8e23-4a0bf1b700c3" />

