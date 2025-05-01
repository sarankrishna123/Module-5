# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
```
regno:212223070023
name:Saran Krishna P S
class Details:
    def __init__(self):
        self.name = input("Enter name: ")
        self.age = input("Enter age: ")

class Employee(Details):
    def __init__(self):
        super().__init__()
        self.emp_id = input("Enter employee ID: ")
        self.department = input("Enter department: ")

    def display_employee(self):
        print("\n--- Employee Details ---")
        print(f"Name: {self.name}")
        print(f"Age: {self.age}")
        print(f"Employee ID: {self.emp_id}")
        print(f"Department: {self.department}")

class Doctor(Details):
    def __init__(self):
        super().__init__()
        self.doctor_id = input("Enter doctor ID: ")
        self.specialization = input("Enter specialization: ")

    def display_doctor(self):
        print("\n--- Doctor Details ---")
        print(f"Name: {self.name}")
        print(f"Age: {self.age}")
        print(f"Doctor ID: {self.doctor_id}")
        print(f"Specialization: {self.specialization}")

print("Enter details for an Employee


```

### OUTPUT  

![image](https://github.com/user-attachments/assets/4ad07138-9114-4173-b814-9eac41d94616)
  


### RESULT
thus the program is executed successfully.
