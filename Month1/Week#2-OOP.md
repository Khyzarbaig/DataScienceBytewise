# Python OOP.

In Python, object-oriented Programming (OOPs) is a programming paradigm that uses objects and classes in programming. It aims to implement real-world entities like inheritance, polymorphisms, encapsulation, etc. in the programming. The main concept of OOPs is to bind the data and the functions that work on that together as a single unit so that no other part of the code can access this data.

## Object Oriented Programming
Let's take an example:
A parrot is an object, as it has the following properties:
•	name, age, colour as attributes
•	singing, dancing as behaviour
The concept of OOP in Python focuses on creating reusable code. This concept is also known as DRY (Don't Repeat Yourself).
So first comes CLASS which is a structure where we define some attributes and class is generic and then we start making OBJECTS which are off course specific and are from class.

## Creating Classes and Objects
### Class
A class is a blueprint for the object.
We can think of class as a sketch of a customer with labels. It contains all the details about the name, member ship type, etc. Based on these descriptions, we can study about the customer.
class Customer:
	def_init_(self, name, membership_type):
	self.name= name
	self.membership_type= membership_type

E.g. 
CLASS: CUSTOMER
Name
Membership type

### Object
An object (instance) is an instantiation of a class. When class is defined, only the description for the object is defined. Therefore, no memory or storage is allocated.

Obj1 = Customer (“Khyzar”,” Gold”)
Obj1 = Customer (“Baig”,” Silver”)
E.g. 
 
OBJECTS
1)Khyzar
Gold

2)Baig
Silver

## Custom Methods
Whenever we want to use the class to change the values or anything related to our object, we use our won methods (Custom Methods)
Custom methods are created in the class block and right below the initializer or constructor method.
E.g. upgrade_membership (self, new_membership):
To invoke this, obj1.upgrade_membership(“Bronze”)
So, it will change the membership status of obj1.
The __init__ method 
The __init__ method is similar to constructors in C++ and Java. It is run as soon as an object of a class is instantiated. The method is useful to do any initialization you want to do with your object. 
 Def_str_(self):
	Print (“converting to string”)
___________________________________________________________________________

## 3 important pillars of OOP
### 1.	Encapsulation
### 2.	Inheritance
### 3.	Polymorphism

These 3 are the “WHY” of OOP.

## 1.	Encapsulation
In encapsulation we can hide the inner details of a class or a certain data and you only share or expose what is needed for the user of the class.
So, suppose we have a field class and instead of people accessing it directly, the will access it through Getters () and Setters () which will give access to data

## 2.	Inheritance
Inheritance allows us to automatically have certain attributes for objects because they are defined in a base class.
Suppose we have a Customer class so a user class under parent (Customer) class will have all the properties defined in its parent class.

## 3.	Polymorphism
Polymorphism in python defines methods in the child class that have the same name as the methods in the parent class. The word polymorphism means having many forms. In programming, polymorphism means the same function name (but different signatures) being used for different types.

