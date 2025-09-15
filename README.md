# DSA-Lab-assignment01
# Name-Yashashvi Kumar
# Roll no.- 2401730122
# Grocery Store Inventory System (C++)

This project implements a simple **Inventory Management System** using array-based data structures in C++.  
It was created as a **Data Structures & Algorithms Lab Assignment** to demonstrate concepts such as **searching, deletion, row-major/column-major traversal, and sparse representation**.

---

## 🚀 Features
- **Add Items**  
  Insert new inventory records (ItemID, ItemName, Quantity, Price).

- **Delete Items**  
  Remove an item from the inventory by its `ItemID`.

- **Search Items**  
  Search by either `ItemID` or `ItemName`.

- **Row-Major & Column-Major Display**  
  - *Row-Major*: Displays each item as a row (ItemID, Price, Quantity).  
  - *Column-Major*: Displays all ItemIDs in one row, all Prices in another, all Quantities in another.

- **Sparse Storage Optimization**  
  Identifies rarely restocked products (items with `Quantity = 0`) and lists them separately.

- **Show All Items**  
  Prints the full inventory in a tabular format.

---

## 📂 Code Structure
- `InventoryItem` – struct that stores:
  - `ItemID` (int)  
  - `ItemName` (string)  
  - `Quantity` (int)  
  - `Price` (float)

- `InventorySystem` – class that manages the inventory.  
  Methods include:
  - `insertItem()` – add a new item  
  - `deleteItem()` – remove item by ID  
  - `searchItem()` / `searchByItem()` – find item by ID or name  
  - `addItemRecord()` / `removeItemRecord()` – aliases for insert/delete  
  - `managePriceQuantity_RowMajor()` – display row-major table  
  - `managePriceQuantity_ColumnMajor()` – display column-major table  
  - `optimizeSparseStorage()` – list items with quantity `0`  
  - `showAllItems()` – print complete inventory  

- `main()` – demonstrates usage by inserting items and printing inventory.

---

## 🛠️ How to Compile and Run
### Using `g++` (Linux/Mac/Windows with MinGW):
```bash
g++ LAB.CPP -o inventory
./inventory
