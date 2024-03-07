# object oriented

### **Class**

A class is a blueprint for creating objects. It defines properties (attributes) and behaviors (methods) that all objects of the class will have.

```python
pythonCopy code
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        print(f"Hello, my name is {self.name} and I'm {self.age} years old.")

```

### **Object**

An object is an instance of a class. It represents a specific entity with its own set of data and behaviors.

```python
pythonCopy code
person1 = Person("Alice", 30)
person2 = Person("Bob", 25)

```

### **Constructor**

A constructor is a special method (**`__init__`** in Python) used to initialize the object's state (attributes) when it is created.

```python
pythonCopy code
def __init__(self, name, age):
    self.name = name
    self.age = age

```

### **Method**

A method is a function defined within a class that performs some action or operation on the object's data.

```python
pythonCopy code
def greet(self):
    print(f"Hello, my name is {self.name} and I'm {self.age} years old.")

```

### **Inheritance**

Inheritance allows a class (subclass) to inherit properties and behaviors from another class (superclass). It promotes code reuse and supports the concept of hierarchy.

```python
pythonCopy code
class Student(Person):
    def __init__(self, name, age, major):
        super().__init__(name, age)
        self.major = major

    def study(self):
        print(f"{self.name} is studying {self.major}.")

```

### **Encapsulation**

Encapsulation refers to the bundling of data (attributes) and methods that operate on the data within a class. It hides the internal state of an object from outside access.

```python
pythonCopy code
class BankAccount:
    def __init__(self, balance=0):
        self.__balance = balance

    def deposit(self, amount):
        self.__balance += amount

    def withdraw(self, amount):
        if amount <= self.__balance:
            self.__balance -= amount
        else:
            print("Insufficient funds.")

```

### **Polymorphism**

Polymorphism allows objects of different classes to be treated as objects of a common superclass. It enables flexibility and code reusability.

```python
pythonCopy code
def show_info(person):
    person.greet()

person1 = Person("Alice", 30)
student1 = Student("Bob", 25, "Computer Science")

show_info(person1)  # Output: Hello, my name is Alice and I'm 30 years old.
show_info(student1)  # Output: Hello, my name is Bob and I'm 25 years old.

```

### **Class Variables and Instance Variables**

Class variables are shared among all instances of a class, while instance variables are unique to each instance.

```python
pythonCopy code
class Dog:
    species = "Canis"

    def __init__(self, name):
        self.name = name

dog1 = Dog("Buddy")
dog2 = Dog("Max")

print(dog1.name)     # Output: Buddy
print(dog2.name)     # Output: Max
print(dog1.species)  # Output: Canis
print(dog2.species)  # Output: Canis

```

```python
class Student
    name = ''
    Student_id = ''

def change_id(self, new_id):
    self.Student_id= new_id

#instansation
stu1 = Student()
stu1.Student_id = 4576
stu1.name='hanna'

stu2 = Student()
stu2.Student_id = 6742
stu2.name='abel'

stu3 = Student()
stu3.Student_id = 6543
stu3.name='gela'

stu4 = Student()
stu4.Student_id = 1234
stu4.name='red'

#stu1.name = 'kebede'  ... this will change the student name

print(stu3)
print(stu1)
```

eg flight

```python
class Flight:
   
   destination =''
   source = ''
   estimated_time  = ''
   passenger_list = []
   capacity = 0
   
   
   def __init__(self, source, destination, capacity):
      
      self.source = source
      self.capacity = capacity
      self.destination  = destination
      
   
   
   
   def add_passenger(self,full_name:str):
      
      if len(self.passenger_list) >= self.capacity:
         print(f'sorry {full_name} the flight is at its max capacity')
      else:
         self.passenger_list.append(full_name)
         print(f'{full_name} has been added to the passengers list ')
   

   def view_passenger(self):
      print(self.passenger_list)
   
   
   def remove_passenger(self, full_name):
      if full_name in self.passenger_list:
         index = self.passenger_list.index(full_name)
         print(f'{full_name} has been removed to the passengers list ')
         
         

flight1 = Flight('ADB','DXB', 5 )

names = ['hanna', 'abel', 'alex', 'berket','mati','dav']

for name in names:
   flight1.add_passenger(name)
   
flight1.view_passenger
```

out put