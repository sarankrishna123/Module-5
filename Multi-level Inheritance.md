# Exp.No:24  
## Multi-level Inheritance

---

### AIM  
To write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.

---

### ALGORITHM

1. Define the `Person` class:
   - Inside the `Person` class, define the `__init__` method (constructor) with two parameters: `name` and `age`.
   - Inside the `__init__` method, assign the `name` to `self.name` and `age` to `self.age`.

2. Define the `PersonDetails` class that inherits from the `Person` class:
   - Inside the `PersonDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `Person` class using `super()` to initialize `name` and `age`.
   - Assign `person_id` to `self.person_id`.

3. Define the `DisplayDetails` class that inherits from the `PersonDetails` class:
   - Inside the `DisplayDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `PersonDetails` class using `super()` to initialize `name`, `age`, and `person_id`.

4. Inside the `DisplayDetails` class, define the `show_details` method:
   - Inside the `show_details` method, return a formatted string with `self.name`, `self.age`, and `self.person_id`.

5. Prompt the user to enter `name` (string), `age` (integer), and `person_id` (integer).

6. Create an instance `person` of the `DisplayDetails` class, passing `name`, `age`, and `person_id` to the constructor.

7. Call the `show_details` method on the `person` object and print the result.

8. Terminate the program.

---

### PROGRAM

```
regno:212223070023
name:Saran Krishna P S
class Person:
    def __init__(self):
        self.name = input("Enter name: ")

class Employee(Person):
    def __init__(self):
        super().__init__()
        self.age = input("Enter age: ")

class Details(Employee):
    def __init__(self):
        super().__init__()
        self.emp_id = input("Enter ID: ")

    def display_info(self):
        print("\n--- Person Details ---")
        print(f"Name: {self.name}")
        print(f"Age: {self.age}")
        print(f"ID: {self.emp_id}")

person_detail = Details()
person_detail.display_info()


```

### OUTPUT
![image](https://github.com/user-attachments/assets/be7749aa-e486-4035-aadd-354f73965605)

### RESULT
thus the program is executed successfully.
