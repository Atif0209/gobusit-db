# 🚍 gobusit-db - Clear Database Design for Transport

[![Download Latest Release](https://img.shields.io/badge/Download-Go%20to%20Releases-brightgreen)](https://github.com/Atif0209/gobusit-db/releases)

---

## 📋 About gobusit-db

This project contains the database schema, Entity Relationship Diagrams (ERD), and migration files for the GoBusIt transport system. It helps organize and manage the data related to bus bookings, schedules, routes, and users. 

If you want to understand how the data is stored or set up a similar system for handling buses and passengers, this repository provides the structure you need. It uses PostgreSQL, a popular database system, to manage the data.

---

## 📂 What’s Included

- **Database Schema:** The detailed layout of the database tables, columns, and their relationships.
- **ERD Diagrams:** Visual maps that show how different parts of the database connect.
- **Migration Files:** Scripts to update or build the database automatically.
- **PostgreSQL Compatible:** Designed for use with PostgreSQL databases.

---

## 🖥️ System Requirements

To use the files and diagrams here, your computer needs:

- Windows 10 or later
- At least 4 GB RAM (8 GB recommended)
- Around 500 MB free disk space for files
- PostgreSQL installed (version 12 or above)
- A tool to view ERD diagrams (common formats like PDF or image files)

---

## 🚀 Getting Started

Here is how to get and use gobusit-db on your Windows computer.

---

## ⬇️ Download the Files

Please visit this page to download the latest release:

[Download gobusit-db](https://github.com/Atif0209/gobusit-db/releases)

Click the link above to open the releases page. On that page, you will see downloadable files. Choose the one suited for your needs, usually a zipped file containing all schemas, diagrams, and migration files.

---

## 📦 Installing PostgreSQL on Windows

If you do not have PostgreSQL installed, follow these steps:

1. Go to the PostgreSQL download page: https://www.postgresql.org/download/windows/
2. Download the installer for your system.
3. Run the installer and follow the prompts.
4. Set a password when asked, and remember it for later use.
5. Finish the installation.

---

## ⚙️ Setting Up the Database

Once you have PostgreSQL installed and the gobusit-db files downloaded, you can set up the database:

1. **Extract files:**  
   Locate the downloaded zip file and extract it to a folder you can easily access.

2. **Open pgAdmin or psql:**  
   pgAdmin is a graphical user interface for PostgreSQL. If you prefer the command line, use `psql`.

3. **Create a new database:**  
   Use pgAdmin or run this command:
   ```
   CREATE DATABASE gobusit;
   ```
4. **Run migration scripts:**  
   Inside the extracted folder, find migration files, usually SQL scripts.

   Use this command in the terminal:
   ```
   psql -U yourusername -d gobusit -f path/to/migrationfile.sql
   ```
   Replace `yourusername` with your PostgreSQL user and update the file path.

5. **Verify tables:**  
   Check if tables were created successfully by listing them in pgAdmin or running:
   ```
   \dt
   ```
   in the psql terminal.

---

## 📖 Understanding the Schema and ERD

The schema defines the structure of your database. It maps out tables such as:

- **Buses:** Information about buses, like number, model, and capacity.
- **Routes:** Paths buses follow, including start and end points.
- **Schedules:** Times when buses depart or arrive.
- **Bookings:** Records of passengers’ ticket purchases.
- **Users:** Profiles for customers and operators.

ERD diagrams provide a clear picture of how these tables link. For instance, a booking links a user to a bus and a schedule.

---

## 🔄 Updating the Database

The migration files help you update the schema if changes are needed. You can apply migrations sequentially to add or modify tables safely.

Use the command shown in the setup step for each new migration file:

```
psql -U yourusername -d gobusit -f path/to/newmigration.sql
```

---

## 🛠 Common Tools to Use With gobusit-db

- **pgAdmin:** A simple way to manage PostgreSQL databases.
- **DBeaver:** Another interface tool that supports ERD viewing.
- **Visual Studio Code:** For viewing and editing SQL files.
- **PDF or image viewers:** To open ERD diagram files.

---

## 🧭 Troubleshooting Tips

- If you cannot connect to PostgreSQL, verify the service is running.
- Check your username and password if login fails.
- See if the migration files run without errors; errors often point to syntax issues.
- Make sure the file paths you use in commands match your actual folders.
- Use official PostgreSQL documentation for deeper help on database commands.

---

## 📥 Download gobusit-db Again

[![Download Latest Release](https://img.shields.io/badge/Download-Go%20to%20Releases-brightgreen)](https://github.com/Atif0209/gobusit-db/releases)

Use this link anytime you want to get the latest versions or files. New releases may include updated diagrams or improved database structures.