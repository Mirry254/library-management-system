# Library Management System  

## 📌 Project Description  
This MySQL-based system helps manage **books, authors, library members, and borrowing records** efficiently. It ensures proper tracking of **which books are available or loaned** while maintaining relationships between books and their authors.  

## ⚡ Features  
- Stores book details, including authors and genres.  
- Maintains a record of **library members**.  
- Tracks **loans**, showing which members borrowed which books.  
- Uses **foreign key constraints** to ensure data integrity.  

## 🏗️ Database Schema  
### **Tables & Relationships**  
- `Authors`: Stores book authors.  
- `Books`: Contains book details, linking to `Authors`.  
- `Members`: Holds library members' details.  
- `Loans`: Tracks book borrowing by members (**One-to-Many** relationship).  

## 📌 ERD Diagram  
the file above is the **Entity Relationship Diagram (ERD)** representing the database structure:

## 🛠️ Setup Instructions  
1. **Import the SQL Schema**  
   - Open MySQL Workbench or phpMyAdmin.  
   - Run `library.sql` to create tables.  

2. **Adding Sample Data (Optional)**  
   - Use `INSERT INTO` statements to test the database.  

3. **Querying the Database**  
   - Retrieve loaned books using:  
     ```sql
     SELECT * FROM Loans WHERE return_date IS NULL;
     ```

## 🔥 How to Push This Project to GitHub  
1. **Initialize Git Repo**:  
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git push origin main
