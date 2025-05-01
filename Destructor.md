# Exp.No:22  
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s2` of the `student` class. When the object `s2` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s2`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM

```
reg no:212223070023
name:Saran Krishna P S
class Student:
    def __init__(self, name):
        self.name = name
        print(f"Student {self.name} has been created.")

    def __del__(self):
        print(f"Student {self.name} has been deleted.")

student1 = Student("John")
del student1


```

### OUTPUT

![image](https://github.com/user-attachments/assets/02e2c9c7-5dc9-438d-94c2-326c6ea6ab16)

### RESULT
thus the program is executed succcessfully.
