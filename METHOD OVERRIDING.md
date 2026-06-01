# Exp.No:26  
## Method Overriding

---

### AIM  
To write a Python program to create a Parent class `Bird` and inherit two child classes `Sparrow` and `Ostrich` from the `Bird` class with the same method `flight()`. Create an object for each class and call the methods of the class which will print the name of the bird that is flying.

---

### ALGORITHM

1. **Begin the program.**
2. **Define the Bird class**:
   - Create a method `intro()` to print "There are many types of birds."
   - Create a method `flight()` to print "Most of the birds can fly but some cannot."
3. **Define the Sparrow class**, which inherits from `Bird`:
   - Override the `flight()` method.
   - Call the `intro()` method from the parent class.
   - Print "Sparrows can fly."
4. **Define the Ostrich class**, which inherits from `Bird`:
   - Override the `flight()` method.
   - Call the `intro()` method from the parent class.
   - Print "Ostriches cannot fly."
5. **Create an object `obj_bird`** of the `Bird` class.
6. **Create an object `obj_spr`** of the `Sparrow` class.
7. **Create an object `obj_ost`** of the `Ostrich` class.
8. **Print the general message** "There are many types of birds."
9. **Call the `flight()` method** on each object (`obj_bird`, `obj_spr`, `obj_ost`) to display the respective messages.
10. **Terminate the program.**

---

### PROGRAM

```
#Reg_no: 212223060288
#Name: Tharun Kumaran G

class Bird:
    def intro(self):
        print("There are many types of birds.")

    def flight(self):
        print("Most of the birds can fly but some cannot.")

class Sparrow(Bird):
    def flight(self):
        super().intro()
        print("Sparrows can fly.")

class Ostrich(Bird):
    def flight(self):
        super().intro()
        print("Ostriches cannot fly.")

obj_bird = Bird()
obj_spr = Sparrow()
obj_ost = Ostrich()

obj_bird.intro()

print("\nBird:")
obj_bird.flight()

print("\nSparrow:")
obj_spr.flight()

print("\nOstrich:")
obj_ost.flight()

```

### OUTPUT

![image](https://github.com/user-attachments/assets/f1055e07-4363-4ed5-94a5-1f694a072306)

### RESULT

The python program to create a Parent class `Bird` and inherit two child classes `Sparrow` and `Ostrich` from the `Bird` class with the same method `flight()` has been executed and verified successfully.
