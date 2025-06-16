
# 🏭 Factory Method Pattern Example – Document Management System

This project demonstrates the **Factory Method Design Pattern** in Java through a simple **Document Management System**. The system supports the creation of different types of documents such as Word, PDF, and Excel using specialized factory classes.

---

## 📌 Overview

The **Factory Method Pattern** provides a way to delegate the instantiation of objects to subclasses. It promotes loose coupling by eliminating the need to bind application-specific classes into the code. In this project, each document type is created via its own factory class, abstracting away the creation logic from the client.

---

## 🗂 Project Structure

```
FactoryMethodPatternExample/
│
├── Document.java               # Document interface
├── WordDocument.java           # Concrete Word document class
├── PdfDocument.java            # Concrete PDF document class
├── ExcelDocument.java          # Concrete Excel document class
│
├── DocumentFactory.java        # Abstract factory class
├── WordDocumentFactory.java    # Factory for Word documents
├── PdfDocumentFactory.java     # Factory for PDF documents
├── ExcelDocumentFactory.java   # Factory for Excel documents
│
└── Main.java                   # Test class (Client code)
```

---

## 🚀 How It Works

1. **`Document`** – An interface defining the methods `open()` and `close()`.
2. **Concrete Document Classes** – `WordDocument`, `PdfDocument`, and `ExcelDocument` implement the `Document` interface.
3. **`DocumentFactory`** – An abstract class declaring the method `createDocument()`.
4. **Concrete Factory Classes** – Each document type has its own factory:

   * `WordDocumentFactory`
   * `PdfDocumentFactory`
   * `ExcelDocumentFactory`
5. **`Main`** – Acts as the client, demonstrating the creation and usage of documents using the factories.

---

## 💡 Sample Output

```
Opening a Word document...
Closing a Word document...
Opening a PDF document...
Closing a PDF document...
Opening an Excel document...
Closing an Excel document...
```

---


