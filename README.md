# iLearning: Community Driven Question & Answer Platform

iLearning is a web-based discussion forum that enables users to ask questions, share knowledge, and participate in community discussions. The platform is inspired by Stack Overflow and provides category-based discussions, user authentication, thread creation, answers, and search functionality.

---

## Features

### User Authentication
- User Registration
- Secure Login System
- Password Hashing
- Session Management
- Logout Functionality

### Discussion Management
- Browse Discussion Categories
- Create New Questions
- Post Answers
- View Question Threads
- Category-Based Organization

### Search
- Search Questions and Discussions
- Full-Text Search Support

### Security
- Password Hashing using PHP Password API
- Prepared Statements (PDO)
- Session-Based Authentication
- Basic Input Validation

---

## Tech Stack

### Frontend
- HTML5
- CSS3
- Bootstrap
- JavaScript

### Backend
- PHP

### Database
- MySQL

### Database Connectivity
- PDO (PHP Data Objects)

---

## Project Structure





---

# Architecture Diagram

```text
                    +------------------+
                    |      User        |
                    +--------+---------+
                             |
                             v
                    +------------------+
                    |    Web Browser   |
                    +--------+---------+
                             |
                             v
                    +------------------+
                    | PHP Application  |
                    +--------+---------+
                             |
        +--------------------+--------------------+
        |                    |                    |
        v                    v                    v

+---------------+   +----------------+   +---------------+
| Authentication|   | Thread Module  |   | Search Module |
+---------------+   +----------------+   +---------------+
        |                    |                    |
        +--------------------+--------------------+
                             |
                             v
                    +------------------+
                    | PDO Layer        |
                    +--------+---------+
                             |
                             v
                    +------------------+
                    | MySQL Database   |
                    +------------------+
                             |
          +------------------+------------------+
          |                  |                  |
          v                  v                  v

    Users Table      Threads Table      Answers Table
                           |
                           v
                    Categories Table
