# 🧩 SliceQL.Core

**SliceQL** is a library that lets you run SQL-like queries directly on multiple Csv files.  
Built with .NET, it supports both command-line usage and a modern web interface.

> ⚠️ Excel (.xlsx) support coming soon!

---

## 🚀 Features

- 📂 Load structured `.txt` or `.csv` files as data sources  
- 🧠 Run SQL queries (`SELECT`, `JOIN`, `WHERE`, etc.) on text files as if they were database tables  
- 💻 Command-line application for advanced users and automation  
- 🌐 ASP.NET Core MVC web interface for easy, interactive usage — **currently deployed on Render**  

---

## 🛠️ Tech Stack

- .NET 8 (C#)  
- Modular design with .NET Class Libraries  
- ASP.NET Core MVC for the web front-end  
- SQLite for query execution and in-memory relational operations 

---

## 📦 Packages Used

- 🧾 System.CommandLine — Modern API for building command-line apps with argument parsing, tab completion, and more  
- 🗃️ System.Data.SQLite — ADO.NET provider for SQLite databases  
- 📊 [DynamicCsvParser](https://github.com/nathan-dauny/CsvToDynamicObject) — Custom library to parse CSV files dynamically and map data types automatically  

---

## ⚙️ Getting Started

### 🌐 Web Interface

Access SliceQL. through this basis front-end for demonstration purpose, hosted on Render:  
[https://sliceql.onrender.com/](https://sliceql.onrender.com/](https://websiteql.onrender.com/)

- Upload multiple CSV files  
- Write and execute SQL queries interactively  
- View results instantly in your browser

### 🔧 Command-Line Usage (Prototype)

```bash
git clone https://github.com/nathan-dauny/SliceQL.git
cd sliceql
dotnet run --project SliceQL/SliceQL.Console -- --data-file "SLiceQL\inputs\tableName.txt" -s "SELECT * FROM tableName;"
