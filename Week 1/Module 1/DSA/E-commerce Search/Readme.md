
#  E-commerce Platform Search Function

This project demonstrates the implementation and performance comparison of **linear search** and **binary search** algorithms in the context of an e-commerce platform's product search system.

---

## 📌 Scenario

You're building a **search feature** for an e-commerce platform that allows users to quickly find products based on their names. Fast performance is critical, especially as the number of products scales.

---

## ✅ Exercise Steps

### 1. Understand Asymptotic Notation

* **Big O Notation** is used to describe the **time complexity** (performance) of an algorithm in terms of input size `n`.

    * Helps developers predict how the algorithm will scale as the dataset grows.

| Case       | Linear Search | Binary Search |
| ---------- | ------------- | ------------- |
| Best Case  | O(1)          | O(1)          |
| Average    | O(n)          | O(log n)      |
| Worst Case | O(n)          | O(log n)      |

---

### 2. Setup

We created a class `Product` with the following attributes:

* `productId`: Unique identifier
* `productName`: Name of the product (used for searching)
* `category`: Category of the product

---

### 3. Implementation

We implemented two search algorithms:

#### 🔹 Linear Search

* Iterates through the list from beginning to end.
* Suitable for **unsorted** product lists.
* ✅ Simple but ❌ slower for large datasets.

#### 🔹 Binary Search

* Requires the list to be sorted by `productName`.
* Continuously halves the search space.
* ✅ Much faster for large datasets.

The product list is stored as:

* A **`List<Product>`** (ArrayList) for dynamic handling.
* Binary search internally sorts the list using `Comparator`.

---

### 4. Analysis

#### 🔸 Time Complexity

| Search Type   | Time Complexity | Requires Sorting? | Suitable for Large Data |
| ------------- | --------------- | ----------------- | ----------------------- |
| Linear Search | O(n)            | ❌ No              | ❌ No                    |
| Binary Search | O(log n)        | ✅ Yes             | ✅ Yes                   |

#### 🔸 Conclusion

Binary search is more efficient and suitable for an e-commerce platform with a **large product catalog**. If the dataset is small or unsorted and performance is not a concern, linear search is a simpler option.

---


## ▶️ How to Run

1. Compile the Java files:

   ```bash
   javac Product.java Main.java
   ```

2. Run the program:

   ```bash
   java Main
   ```

---

## 📄 Sample Output

```
Linear Search Result: Product{productId=3, productName='Phone', category='Electronics'}
Binary Search Result: Product{productId=3, productName='Phone', category='Electronics'}
```

---


