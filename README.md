# 📚 SQL Project — Book Service Analysis

> Data analysis project using SQL to explore a book service database and extract insights to support the development of a value proposition for a new product in the digital reading market.

---

## 🛠️ Tools & Technologies

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 📫 Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bladimir-andres-hernandez-a1764a2b7)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:bladimir4hernandez@gmail.com)

---

## 📌 Project Overview

A book subscription startup is entering a highly competitive market. To define its value proposition, the company needs to understand the current landscape of books, authors, publishers, and user behavior.

This project connects to a **PostgreSQL database** using SQLAlchemy and Python, and runs advanced SQL queries to extract business insights across 5 related tables: `books`, `authors`, `publishers`, `ratings`, and `reviews`.

---

## 🗄️ Database Structure

```
books        → book_id, title, author_id, publisher_id, num_pages, publication_date
authors      → author_id, author
publishers   → publisher_id, publisher
ratings      → rating_id, book_id, username, rating
reviews      → review_id, book_id, username, text
```

---

## 🎯 Key Questions Answered

- How many books were published after January 1, 2000?
- Which books have the most reviews and highest average ratings?
- Which publisher has produced the most books with over 50 pages?
- Which author has the highest average rating (with at least 50 ratings)?
- How many text reviews do the most active users write on average?

---

## 🔍 SQL Techniques Used

```
- Aggregate functions: COUNT, AVG
- Filtering: WHERE, HAVING
- Table joining: JOIN, LEFT JOIN (across 5 tables)
- Common Table Expressions (CTEs): WITH
- Subqueries and nested queries
- Sorting and limiting: ORDER BY, LIMIT
- Connected to a real PostgreSQL database via SQLAlchemy
```

---

## 📊 Key Findings & Conclusions

### 📖 Books & Publications
- **819 books** were published after January 1, 2000, showing the catalog is largely composed of modern titles — useful for targeting contemporary readers.

### ⭐ Ratings & Reviews
- Most books have **2–3 written reviews**, with average ratings ranging from **1.5 to 5.0**.
- Books with higher average ratings are strong candidates for recommendations and promotion.

### 🏆 Top Publisher
- **Penguin Books** leads with **42 substantial titles** (over 50 pages), making it the most impactful publisher in the catalog.

### ✍️ Top Author
- **J.K. Rowling / Mary GrandPré** achieved the highest average rating of **4.28**, based on books with at least 50 ratings — consistently well-received across the platform.

### 👤 Active Users
- Users who rated more than 50 books write an average of **24.33 text reviews**, indicating a highly engaged user base whose opinions are key for content recommendations.

---

## 📁 Project Structure

```
📦 sql-book-service-analysis
 ┣ 📓 SQL_Project___Book_Service_Analysis.ipynb   # Main notebook with all queries
 ┗ 📄 README.md
```

---

⭐ *If you found this project useful, feel free to leave a star!*
