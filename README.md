#             Java and Kotlin Interview Questions and Answers
# This repository contains common Java and Kotlin interview questions with detailed answers. These questions are tailored for developers preparing for technical interviews, particularly for Android development roles. Topics include OOP principles, memory management, multithreading, coroutines, and Kotlin-specific features

 # Table of Contents 
# 1.  Four Principles of OOP
# 2.  Difference Between an Interface and an Abstract Class in Java
# 3.  Purpose of val and var in Kotlin
# 4.  Java Memory Management
# 5.  Kotlin Extension Functions
# 6.  Synchronous vs Asynchronous Programming
# 7.  Kotlin Null Safety
# 8.  What is a Coroutine in Kotlin
# 9.  Multithreading in Java
# 10.  Difference Between launch and async in Kotlin Coroutines
# 11.  Purpose of suspend Function in Kotlin
# 12.  Kotlin and Java Interoperability
# 13.  Conclusion

# 1. Four Principles of OOP
Question: What are the four principles of OOP?
# Answer:

The four principles of Object-Oriented Programming (OOP) are:

- Encapsulation: Hiding internal states and behaviors, only exposing a public interface.
Example: Private variables with public getters/setters.

- Abstraction:
- Simplifying complex systems by modeling classes relevant to the problem.
- **Example:**
-  Payment method interface with implementations like CreditCard, PayPal.

- Inheritance: Creating new classes by inheriting properties from existing ones.
Example: Dog inherits from Animal.

- Polymorphism: Allowing objects to be treated as instances of their parent class.
Example: A method can accept both Circle and Rectangle as they implement Shape.


# 2. Difference Between an Interface and an Abstract Class in Java
# Question:
What is the difference between an interface and an abstract class in Java?

# Answer:

 - **Interface:**
 - All methods are abstract by default (Java 8+ allows default methods).
 - Can be implemented by multiple classes (supports multiple inheritance).

- **Abstract Class**
- Can have both abstract and concrete methods.
-  A class can only inherit from one abstract class, but can implement multiple interfaces.




