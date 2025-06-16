
# SingletonPatternExample - Logger

This project demonstrates the **Singleton Design Pattern** using a simple `Logger` class in Java.

##  What is the Singleton Pattern?

The **Singleton Pattern** ensures that a class has **only one instance** and provides a global point of access to it. It is useful when exactly one object is needed to coordinate actions across the system—like a logger, configuration manager, or cache.

## 📂 Project Structure

```bash
SingletonPatternExample/
├── Logger.java    # Singleton Logger class
└── Test.java      # Demonstration and testing of Logger behavior
```

## 📄 Logger.java

The `Logger` class demonstrates:

* **Lazy Initialization**: Instance is created only when needed.
* **Private Constructor**: Restricts instantiation from other classes.
* **Static Access Method**: Provides global access via `getLogInstance()`.

```java
Logger logger1 = Logger.getLogInstance();
logger1.log("First log message");
```

## 📄 Test.java

This class tests the singleton behavior:

* It gets two logger instances and logs messages.
* It checks whether both instances point to the **same object** (i.e., singleton behavior).

### Sample Output:

```
Logger initialized
Log message: First log message
Log message: Second log message
Both logger instances are the same.
```

## ✅ Key Concepts Demonstrated

* **Singleton Pattern**
* **Lazy Initialization**
* **Object Identity Validation**
* **Single Responsibility Principle** (for logging)

## 🚀 How to Run

1. Compile the Java files:

   ```bash
   javac Logger.java Test.java
   ```

2. Run the `Test` class:

   ```bash
   java Test
   ```


