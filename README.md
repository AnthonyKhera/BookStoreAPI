# Book Store API | GeekText

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies](#technologies)
- [Usage](#usage)

## Introduction
Welcome to the Book Store API, also known as GeekText! This project showcases the creation of a robust REST API with CRUD features designed to manage a book store database. Our primary objectives are to empower administrators to add books and authors to the store and enable users to explore the collection and make book purchases.

## Features
This application supports the following features.
- Add books to the store.
- Manage authors in the database.
- Browse and search for books by genre, best sellers, average rating, and authors.
- Create and manage user accounts with username, password, email address, credit card info, and shipping address.
- Build and maintain a unique cart, displaying book information and the cart's total price.
- Write comments and leave ratings for books.
- View all comments and the average rating for a selected book.

## Technologies
This project leverages the following technologies:
- Java
- Spring Boot / Spring Framework
- PostgreSQL
- Postman for API testing
- IntelliJ IDEA as the integrated development environment (IDE)
- Git for version control

## Usage

Example requests to interact with the Book Store API:

1. **Get All Books**
   - **HTTP Method:** GET
   - **Endpoint:** `/bookstore/getAllBooks`

2. **Get Top Sellers**
   - **HTTP Method:** GET
   - **Endpoint:** `/bookstore/topSellers`

3. **Get Books by Genre**
   - **HTTP Method:** GET
   - **Endpoint:** `/bookstore/browseByGenre`
   - **Parameters:** `genre` (e.g., `/bookstore/browseByGenre?genre=Mystery`)

4. **Get Books by Author**
   - **HTTP Method:** GET
   - **Endpoint:** `/bookstore/getBookByAuthor`
   - **Parameters:** `author_last` (e.g., `/bookstore/getBookByAuthor?author_last=King`)

5. **Add New Author**
   - **HTTP Method:** POST
   - **Endpoint:** `/bookstore/addAuthor`
   - **Parameters:** `author_num`, `author_bio`, `author_first`, `author_last`

6. **Add New Book**
   - **HTTP Method:** POST
   - **Endpoint:** `/bookstore/addBook`
   - **Parameters:** `book_code`, `author_num`, `title`, `publisher_code`, `price`, `genre`, `year_pub`, `copies_sold`, `book_description`, `average_rating`

7. **Add Review**
   - **HTTP Method:** POST
   - **Endpoint:** `/bookstore/addReview`
   - **Parameters:** `reviewID`, `bookCode`, `userID`, `rating`, `comment`, `datestamp`

8. **Get Average Rating for a Book**
   - **HTTP Method:** GET
   - **Endpoint:** `/bookstore/getAvgRating`
   - **Parameters:** `bookCode` (e.g., `/bookstore/getAvgRating?bookCode=12345`)

9. **Add Item to Cart**
   - **HTTP Method:** POST
   - **Endpoint:** `/bookstore/addItem`
   - **Parameters:** `userId`, `bookCode`

10. **Remove Item from Cart**
    - **HTTP Method:** DELETE
    - **Endpoint:** `/bookstore/removeItem`
    - **Parameters:** `userId`, `bookCode`


