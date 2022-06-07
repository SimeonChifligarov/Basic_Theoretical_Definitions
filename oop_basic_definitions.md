
# (What is an) Object?
 - Object is a data abstraction - an internal representation and an interface
 - The internal representation - should be private
 - The interface - defines behaviors but hides implementation

# Class Objects
 - Classes support two kinds of operations:
    - attribute references – access them using the "." operator 
    - instantiation - uses function notations

# "self" Parameter
 - self is used to represent the (current) instance of the class
 - binds the attributes with the given arguments
 - not a keyword, but using it increases code readability

# Instance Objects
 - Instances support only one kind of operations:
    - attribute references - access them using the "." operator 


# Polymorphism
	[...]

 # Run-Time Polymorphism
    - A subclass can override a method of its superclass
	[...]

 # Compile-Time Polymorphism
    - Python does not support compile-time polymorphism or method overloading
    - If a class has multiple methods with the same name,
	the method defined in the last will override the earlier one
	[...]

# Duck Typing 
	[...]

 - Duck typing is a concept related to dynamic typing, where the type or the class of an object
    is less important than the methods it defines.
    When you use duck typing, you do not check types at all.
    Instead, you check for the presence of a given method or attribute.

# Monkey Patching
 - A monkey patch (also spelled monkey-patch, MonkeyPatch) is a way to extend or modify
    the runtime code of dynamic languages (e.g. Smalltalk, JavaScript, Objective-C, Ruby, Perl, Python, Groovy, etc.)
    without altering the original source code.

 - Monkey patching can only be done in dynamic languages, of which Python is a good example.
    Changing a method at runtime instead of updating the object definition is one example;
    similarly, adding attributes (whether methods or variables) at runtime is considered monkey patching.

 - In Python, the term monkey patch refers to dynamic (or run-time) modifications of a class or module.
    In Python, we can actually change the behavior of code at run-time.

# LSP
	[...]

# Iterators
	[...]


 - An Iterable is basically an object that any user can iterate over.
    An Iterator is also an object that helps a user in iterating over another object (that is iterable).
    We can generate an iterator when we pass the object to the iter() method.
 - Note that every iterator is also an iterable, but not every iterable is an iterator.
    For example, a list is iterable but a list is not an iterator.
    An iterator can be created from an iterable by using the function iter()

 - The Iteration Protocol in Python
    - Essentially, the protocol is consisted of two object types, namely iterable and iterator.
       The iterable object is the one you iterate over its elements.
       The iterator object is the one that produces the values during the iteration
       and it also being returned by the iterable object.

# Generators
    - Way of Creating Iterators
 - Generators are a simple way of creating iterators
 - A function that returns an object (iterator)
 - (This) iterator could later be iterated over (one value at a time)


# yield Statement
	[...]

# Generators vs Normal Functions
	[...]

# Generator Expression
	[...]

# Closure
	[...]

# Decorators
	[...]

# functools.wraps()
	[...]

 - from functools import wraps

def uppercase(function):
    @wraps(function)
    def wrapper():
        result = function()
        uppercase_result = result.upper()
        return uppercase_result

    return wrapper

# Classes as Decorators
 - We can also use classes as decorators
 - We usually do that when we need to maintain a state
 - To use a class as a decorator, we need to implement the __call__ method
 - The __call__ method allows class instances to be called as functions

class Fibonacci:
    def __init__(self):
        self.cache = {}

    def __call__(self, n):
        if n not in self.cache:
            if n == 0:
                self.cache[0] = 0
            elif n == 1:
                self.cache[1] = 1
            else:
                self.cache[n] = self(n-1) + self(n-2)
        return self.cache[n]


# Design Patterns
	[...]

 - Patterns solve software structural problems like
    - Abstraction
    - Encapsulation
    - Separation of concerns
    - Coupling and cohesion
    - Separation of interface and implementation

 - Elements of a Design Pattern
    - Pattern name
	[...]
    - Problem
	[...]
    - Solution
	[...]
    - Consequences
	[...]

### Types of Design Patterns
 - Creational patterns
	Deal with initialization and configuration of classes and objects
 - Structural patterns
	Describe ways to assemble objects to implement new functionality
	Composition of classes and objects
 - Behavioral patterns
	Deal with dynamic interactions among societies of classes
	Distribute responsibility

 - Creational patterns
Singleton, Simple Factory, Factory Method, Abstract Factory, Builder,
Prototype, Fluent Interface, Object Pool, Lazy Initialization

 - Structural Patterns
Façade, Composite, Flyweight, Proxy, Decorator, Adapter, Bridge

 - Behavioral Patterns
Chain of Responsibility, Iterator, Command, Template Method, Strategy,
Observer, Mediator, Memento, State, Interpreter, Visitor


# Memoization
 - Memoization is a specific form of caching that involves caching the return value of a function based on its parameters (?).
 - Caching is a more general term; for example, HTTP caching is caching but not memoization.
