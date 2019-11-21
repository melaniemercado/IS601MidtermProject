### Python Definitions:

1) How Python uses Indentation to control Flow:
    Python uses whitespace (i.e. indentation) to delimit scope:
Its rules are that: One or more whitespace characters (spaces or tabs) is sufficient to serve as indentation. A given indented block must use a uniform level of indentation.

2) Don't Repeat Yourself:
    Don't repeat yourself (DRY, or sometimes do not repeat yourself) is a principle of software development aimed at reducing repetition of software patterns,[1] replacing it with abstractions or using data normalization to avoid redundancy.

3) Design Patterns from Gang of Four:
    The GoF Design Patterns are broken into three categories: Creational Patterns for the creation of objects; Structural Patterns to provide relationship between objects; and finally, Behavioral Patterns to help define how objects interact.


4) Class:
    A class is a code template for creating objects. Objects have member variables and have behaviour associated with them. In python a class is created by the keyword class . An object is created using the constructor of the class. This object will then be called the instance of the class

5) Object:
    Python is an object oriented programming language. Unlike procedure oriented programming, where the main emphasis is on functions, object oriented programming stress on objects. Object is simply a collection of data (variables) and methods (functions) that act on those data. And, class is a blueprint for the object

6) Static:
    Static means, that the member is on a class level rather on the instance level. Static variables exist only in single instance per class and are not instantiated. If a static variable is changed in one instance of the class, the change will affect its value in all other instances.


7) Property / Attribute:
    Attributes are described by data variables for example like name, age, height etc. Properties are special kind of attributes which have getter, setter and delete methods like __get__, __set__ and __delete__ methods. ... In Python, you can define getters, setters, and delete methods with the property function.
8) Method:
    In Python, a method is a function that is available for a given object because of the object's type.

9) Exception:

    An exception is a breakpoint that can be set on executable lines of code. This allows you to suspend program execution at a specific point and examine its behavior.

10) Unit Test:

    A unit test is a way of testing a unit - the smallest piece of code that can be logically isolated in a system. In most programming languages, that is a function, a subroutine, a method or property. Unit testing involves breaking your program into pieces, and subjecting each piece to a series of tests.

11) Constructor: 

    A constructor is a special kind of method that Python calls when it instantiates an object using the definitions found in your class. Python relies on the constructor to perform tasks such as initializing(assigning values to) any instance variables that the object will need when it starts. Constructors can also verify that there are enough resources for the object and perform any other start-up task you can think of.

    The name of a constructor is always the same, __init__(). The constructor can accept arguments when necessary to create the object. When you create a class without a constructor, Python automatically creates a default constructor for you that doesn’t do anything. Every class must have a constructor, even if it simply relies on the default constructor. 

12) Factory:

    Factory Method is a creational design pattern used to create concrete implementations of a common interface. It separates the process of creating an object from the code that depends on the interface of the object.
    
    For example, an application requires an object with a specific interface to perform its tasks. The concrete implementation of the interface is identified by some parameter.
    Instead of using a complex if/elif/else conditional structure to determine the concrete implementation, the application delegates that decision to a separate component that creates the concrete object. With this approach, the application code is simplified, making it more reusable and easier to maintain.

13) Decorator:

    A decorator is a design pattern in Python that allows a user to add new functionality to an existing object without modifying its structure. Decorators are usually called before the definition of a function you want to decorate.

    Decorators are very powerful and useful tool in Python since it allows programmers to modify the behavior of function or class. Decorators allow us to wrap another function in order to extend the behavior of wrapped function, without permanently modifying it.

14) Extend Class:

    Inheritance is the mechanism of deriving new classes from existing ones. By doing this we get a hierarchy of classes. In most class-based object-oriented languages, an object created through inheritance (a "child object") acquires all, - though there are exceptions in some programming languages, - of the properties and behaviors of the parent object.

    Inheritance allows programmers to create classes that are built upon existing classes, and this makes it possible that a class created through inheritance inherites the attributes and methods of the parent class. This means that inheritance supports code reusability. The methods or generally speaking the software inherited by a subclass is considered to be reused in the subclass. The relationships of objects or classes through inheritance give rise to a directed graph.

15) CSV Files:

    CSV (Comma Separated Values) is a simple file format used to store tabular data, such as a spreadsheet or database. A CSV file stores tabular data (numbers and text) in plain text. Each line of the file is a data record. Each record consists of one or more fields, separated by commas. The use of the comma as a field separator is the source of the name for this file format.
