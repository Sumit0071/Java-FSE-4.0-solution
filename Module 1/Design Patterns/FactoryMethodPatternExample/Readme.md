# 🏭 Factory Method Pattern Example - Document Management System

This project demonstrates the **Factory Method Design Pattern** in Java. The use case is a **Document Management System** that creates different types of documents (Word, PDF, Excel) using factory classes.

---

## 📌 Overview

The **Factory Method Pattern** allows the instantiation of objects without exposing the creation logic to the client. Instead, it uses factory classes to delegate the responsibility of creating specific types of documents.

---

## 🗂 Project Structure

FactoryMethodPatternExample/
│
├── Document.java # Document interface
├── WordDocument.java # Concrete Word document class
├── PdfDocument.java # Concrete PDF document class
├── ExcelDocument.java # Concrete Excel document class
│
├── DocumentFactory.java # Abstract factory class
├── WordDocumentFactory.java # Word document factory
├── PdfDocumentFactory.java # PDF document factory
├── ExcelDocumentFactory.java # Excel document factory
│
└── Main.java # Test class


---

## 🚀 How It Works

1. `Document` is an interface that defines the `open(), close()` method.
2. `WordDocument`, `PdfDocument`, and `ExcelDocument` implement the `Document` interface.
3. `DocumentFactory` is an abstract class with the method `createDocument()`.
4. Each document type has its own factory class:
    - `WordDocumentFactory`
    - `PdfDocumentFactory`
    - `ExcelDocumentFactory`
5. The `Main` class tests the creation of documents through the factories.

---

## 💡 Sample Output

Opening a Word document...
Closing a Word document...
Opening a pdf document ...
Closing a pdf document...
Opening an excel document ...
Closing an excel document...
