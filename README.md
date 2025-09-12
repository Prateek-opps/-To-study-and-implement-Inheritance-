EXPERIMENT - 14

Prateek Sinha

24070123077

ENTC A3

# Inheritance in C++

This project demonstrates the concept of **Inheritance in C++** with examples of:
- Single Inheritance  
- Multiple Inheritance  
- Multilevel Inheritance  
- Hierarchical Inheritance
- Access Specifiers

---

##  Theory

###  Single Inheritance
- In single inheritance, a **derived class** inherits from **only one base class**.  
- It models an **“is-a” relationship** between base and derived classes.  
- Example: A `Student` **is a** `Person`.  

###  Multiple Inheritance
- In multiple inheritance, a class can inherit from **more than one base class**.  
- It is useful when a new class requires features from different unrelated classes.  
- Example: A `Car` can inherit from both `Vehicle` and `Engine`.  

###  Multilevel Inheritance
- In multilevel inheritance, a class is derived from another derived class.  
- This creates a chain of inheritance, passing features across multiple levels.  
- Example: `LivingBeing → Animal → Dog`.  

###  Hierarchical Inheritance
- In hierarchical inheritance, multiple classes inherit from a **single base class**.  
- Example: `Smartphone`, `Laptop`, and `Smartwatch` all inherit from `Gadget`.

### Access Specifiers
- `public`: Accessible by everyone.  
- `protected`: Accessible within the class and derived classes.  
- `private`: Accessible only within the class itself.

In this project:
- `startEngine()` is public in `Vehicle`.  
- `stopEngine()` is private in `Vehicle`, but accessible indirectly using `tryStopEngine()`.  
- `showSpecs()` is protected in `Car`, used by `ElectricCar`.

---

##  Algorithm

###  Single Inheritance
1. Define a base class with attributes and methods.  
2. Define a derived class inheriting from the base.  
3. Add extra members to the derived class.  
4. Create an object of the derived class and access both base and derived members.  

###  Multiple Inheritance
1. Define two or more base classes with their own attributes/methods.  
2. Define a derived class inheriting from all base classes.  
3. Add new members to the derived class.  
4. Create an object of the derived class and access all inherited features.  

###  Multilevel Inheritance
1. Define a base class with basic features.  
2. Define a derived class inheriting the base and add new features.  
3. Define another class inheriting the derived class and add more features.  
4. Create the final derived class object and access all features.  

###  Hierarchical Inheritance
1. Define a single base class with common features.  
2. Define multiple derived classes inheriting from the base.  
3. Each derived class adds its own unique features.  
4. Create objects of all derived classes and access base + derived features.

### Access Specifiers
1. **Define Base Class `Vehicle`:**  
    - Implement methods to start and stop the engine.  
    - Provide a public method `tryStopEngine()` to safely call `stopEngine()`.

2. **Define Derived Class `Car`:**  
    - Attributes: `fuelType`, `horsepower`, `seats`, and `model`.  
    - Constructor takes user input for fuel type, horsepower, and seats.  
    - Protected method `showSpecs()` displays car specifications.

3. **Define Derived Class `ElectricCar`:**  
    - Additional attribute `batteryCapacity`.  
    - Constructor takes input for battery capacity.  
    - Public method `display()` shows car and battery specs.

4. **Use in `main()`:**  
    - Create a `Car` object and call `startEngine()` and `tryStopEngine()`.  
    - Create an `ElectricCar` object and call `startEngine()` and `display()`.
   
---

##  Conclusion
- **Single Inheritance** shows how a class can reuse one base class.  
- **Multiple Inheritance** combines features from multiple base classes.  
- **Multilevel Inheritance** demonstrates inheritance across multiple levels.  
- **Hierarchical Inheritance** shows how many derived classes can share the same base.  





