# 🎬 Movie Ticket Booking System --- MySQL SQL Project

A MySQL-based relational database project for managing customers,
movies, theatres, and movie ticket bookings.

This project demonstrates SQL concepts including database design,
primary keys, foreign keys, constraints, data retrieval, filtering,
sorting, aggregate functions, JOINs, GROUP BY, HAVING, and subqueries.

------------------------------------------------------------------------

## 📌 Project Overview

The Movie Ticket Booking System represents a basic movie ticket booking
workflow using a relational database.

The database contains four main entities:

-   👤 Customers
-   🎬 Movies
-   🏢 Theatres
-   🎟️ Bookings

The `bookings` table connects customers, movies, and theatres through
foreign-key relationships.

The project includes SQL queries ranging from basic data retrieval to
more advanced analysis of booking records, revenue, movies, theatres,
and customer activity.

------------------------------------------------------------------------

## ✨ Features

-   👤 Customer information management
-   🎬 Movie information management
-   🏢 Theatre information management
-   🎟️ Movie ticket booking records
-   💰 Ticket revenue analysis
-   💳 Payment-method analysis
-   📊 Booking and customer analysis
-   🔎 Data filtering and sorting
-   🔗 Multi-table analysis using JOINs
-   📈 SQL analysis using aggregate functions, subqueries, and grouping

------------------------------------------------------------------------

## 🎯 Objectives

-   Designing a relational database using MySQL
-   Creating related tables
-   Applying Primary Key and Foreign Key relationships
-   Maintaining referential integrity
-   Storing customer, movie, theatre, and booking information
-   Practicing SQL filtering and sorting
-   Performing aggregate analysis
-   Using JOINs across multiple tables
-   Applying GROUP BY and HAVING
-   Writing subqueries
-   Answering practical movie-booking business questions

------------------------------------------------------------------------

## 🗄️ Database Structure

**Database:** `movie_booking_db`

  Table         Purpose
  ------------- -----------------------------------
  `customers`   Stores customer information
  `movies`      Stores movie information
  `theatres`    Stores theatre information
  `bookings`    Stores ticket booking information

### Customers

  Column            Description
  ----------------- ----------------------------
  `customer_id`     Unique customer identifier
  `customer_name`   Customer name
  `gender`          Customer gender
  `city`            Customer city
  `signup_date`     Customer signup date

### Movies

  Column               Description
  -------------------- ---------------------------
  `movie_id`           Unique movie identifier
  `movie_name`         Movie name
  `genre`              Movie genre
  `language`           Movie language
  `duration_minutes`   Movie duration in minutes

### Theatres

  Column           Description
  ---------------- ---------------------------
  `theatre_id`     Unique theatre identifier
  `theatre_name`   Theatre name
  `city`           Theatre city
  `total_seats`    Total theatre seats

### Bookings

  Column             Description
  ------------------ ---------------------------
  `booking_id`       Unique booking identifier
  `customer_id`      Customer reference
  `movie_id`         Movie reference
  `theatre_id`       Theatre reference
  `show_date`        Movie show date and time
  `seats_booked`     Number of seats booked
  `ticket_amount`    Booking amount
  `booking_status`   Booking status
  `payment_method`   Payment method

------------------------------------------------------------------------

## 🔗 ER Diagram & Database Relationships

The ER diagram represents the four tables in the Movie Ticket Booking
System, including their attributes and relationships.

![Movie Booking Database ER Diagram](ER-Daigram.jpeg)

### Database Relationships

-   **Customers → Bookings:** One customer can make multiple bookings.
-   **Movies → Bookings:** One movie can appear in multiple bookings.
-   **Theatres → Bookings:** One theatre can have multiple bookings.

The `bookings` table connects customers, movies, and theatres through
foreign keys.

------------------------------------------------------------------------

## 📊 SQL Queries

The project contains 60 SQL analysis queries divided into three files.

  File                   Description
  ---------------------- -----------------------------
  `Simple_Queries.sql`   20 basic SQL queries
  `Medium_Queries.sql`   20 intermediate SQL queries
  `Hard_Queries.sql`     20 advanced SQL queries

These queries are designed to practice SQL concepts and analyze movie
bookings, ticket amounts, customer activity, and theatre performance.

------------------------------------------------------------------------

## 🛠️ Technologies Used

-   **Database:** MySQL
-   **Tool:** MySQL Workbench
-   **Language:** SQL
-   **Version Control:** Git and GitHub

------------------------------------------------------------------------

## 🚀 How to Use

1.  Clone or download this repository.
2.  Open MySQL Workbench and connect to your MySQL server.
3.  Open `movie_booking_db.sql`.
4.  Execute the script to create and populate the database.
5.  Open the Simple, Medium, and Hard query files.
6.  Execute the queries to explore the database and analyze the results.

------------------------------------------------------------------------

## 👩‍💻 Author

Created as a MySQL database project to practice relational database
design and SQL query analysis.
