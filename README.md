#             Java and Kotlin Interview Questions and Answers
# This repository contains common Java and Kotlin interview questions with detailed answers. 
These questions are tailored for developers preparing for technical interviews, particularly for Android development roles. Topics include OOP principles, memory management, multithreading, coroutines, and Kotlin-specific features

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

- **Encapsulation:**
-  Hiding internal states and behaviors, only exposing a public interface.
- **Example:**
- Private variables with public getters/setters.

- Abstraction:
- Simplifying complex systems by modeling classes relevant to the problem.
- **Example:**
-  Payment method interface with implementations like CreditCard, PayPal.

- **Inheritance:**
- Creating new classes by inheriting properties from existing ones.
- **Example:**
-  Dog inherits from Animal.

- **Polymorphism:**
-  Allowing objects to be treated as instances of their parent class.
  - **Example:**
- A method can accept both Circle and Rectangle as they implement Shape.


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

 # 3. Purpose of val and var in Kotlin
 # Answer:
 - val: Declares an immutable variable, equivalent to final in Java.
- **Example:**
  ``` kotlin
  val name = "John"
    ```

- var: Declares a mutable variable that can be reassigned.
- **Example:**
 ``` kotlin
  var age = 30
  ```

# 4. Java Memory Management
# Question: 
 How does Java handle memory management?
# Answer:

- Java uses Garbage Collection (GC) to automatically manage memory.
- Unreferenced objects are removed from memory to prevent memory leaks.
- Java divides memory into Heap (for object storage) and Stack (for references).

 # 5. Kotlin Extension Functions
# Question:
What are Kotlin's extension functions?
# Answer:
Extension functions let you add functionality to existing classes without modifying their code.
``` kotlin
fun String.reverseText(): String {
    return this.reversed()
}

val original = "Hello"
println(original.reverseText()) // Output: olleH
```

# 6.Synchronous vs Asynchronous Programming

# Question:
What is the difference between synchronous and asynchronous programming in Java and Kotlin?

# Answer:
- **Synchronous Programming:**
  - Code runs in sequence, blocking further execution until the current task finishes.
  
- **Asynchronous Programming:**
  - Allows other operations to execute while waiting for a task to complete.
  - In Kotlin, coroutines simplify asynchronous programming compared to Java’s threading model.


# 7. Kotlin Null Safety

## Question:
How does Kotlin ensure null safety?

## Answer:
- Kotlin enforces null safety by default, preventing `NullPointerException`.
- Variables are non-nullable unless explicitly marked with a `?` (e.g., `String?`).

 ```kotlin
val name: String? = null
println(name?.length) // Safe call
 ```

## 8. What is a Coroutine in Kotlin
## Question:
What is a coroutine in Kotlin?

## Answer:
- A coroutine is Kotlin's lightweight thread for asynchronous programming.
- They can suspend and resume execution without blocking the main thread.

# 9. Multithreading in Java
# Question:
How do you handle multithreading in Java?
# Answer:
- In Java, you can create a new thread by extending Thread or implementing Runnable.

```java
class MyTask implements Runnable {
    public void run() {
        System.out.println("Task is running");
    }
}

Thread thread = new Thread(new MyTask());
thread.start();
```
# 10. Difference Between launch and async in Kotlin Coroutines
# Question:
What is the difference between launch and async in Kotlin Coroutines?
# Answer:
- launch: Starts a coroutine that does not return a result.
- async: Starts a coroutine that returns a Deferred result, which can be accessed using await().
```kotlin
val job = launch { 
    // No result
}
val deferred = async {
    "Hello"
}
println(deferred.await()) // Prints "Hello"
```
# 11. Purpose of suspend Function in Kotlin
# Question: 
What is the purpose of the suspend function in Kotlin?
# Answer:
- A suspend function can be paused and resumed without blocking the thread.
- It’s used in coroutines for tasks like network requests.
  
```kotlin
suspend fun fetchData() {
    delay(1000)
    println("Data fetched")
}
```

# 12. Kotlin and Java Interoperability
# Question: 
How does Kotlin handle interoperability with Java?
# Answer:
- Kotlin is fully interoperable with Java. Kotlin code can call 
- Java code and vice versa.
 ```kotlin
  val list = ArrayList<String>() // Using Java's ArrayList
list.add("Hello")
```

# 13. Conclusion
By preparing for these common Java and Kotlin interview questions, you'll be equipped to handle the technical sections of your interview with confidence. Understanding the nuances of each language, such as Kotlin’s null safety and coroutines, will give you an edge in Android development and backend roles.

