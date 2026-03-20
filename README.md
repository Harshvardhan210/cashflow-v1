# <p align="center">💰 Cashflow</p>

<p align="center">
  <img src="images/logo.png" alt="Cashflow Logo" width="200">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Spring%20Boot-4.0.0-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot">
  <img src="https://img.shields.io/badge/Java-21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java 21">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white" alt="JWT">
</p>

<p align="center">
  <strong>A modern, powerful, and secure personal finance tracking application.</strong>
</p>

---

## 🌟 Overview

**Cashflow** is a sleek and efficient backend service built with **Spring Boot 4** and **Java 21**. It empowers users to manage their daily expenses, track their spending habits, and maintain full control over their financial health. With integrated **JWT** and **OAuth2 (Google)** authentication, your financial data stays secure and accessible only to you.

---

## 🚀 Key Features

- 🔐 **Secure Authentication**: Traditional Login/Register with JWT tokens + Google OAuth2 integration.
- 💳 **Expense Management**: Full CRUD operations for tracking expenses.
- 👤 **User-Specific Data**: Each user has their own isolated financial records.
- 🐳 **Docker Ready**: Easily containerize and deploy your application.
- 📊 **Scalable Architecture**: Built using Spring Boot best practices, ready for growth.

---

## 🛠 Tech Stack

- **Framework**: Spring Boot 4.0.0 (Experimental)
- **Language**: Java 21 (LTS)
- **Persistence**: Spring Data JPA + PostgreSQL
- **Security**: Spring Security + JJWT + OAuth2 Client
- **Utility**: Lombok (for clean, boilerplate-free code)
- **Containerization**: Docker

---

## ⚙️ Getting Started

### 📋 Prerequisites

- **JDK 21** installed.
- **PostgreSQL** instance running.
- **Maven** (optional, `mvnw` wrapper included).

### 🛠 Configuration

1.  **Database Setup**: Create a database named `cashFlow` in your PostgreSQL instance.
2.  **Environment Variables**: Update `src/main/resources/application.properties` or set the following environment variables:

    ```bash
    DB_URL=jdbc:postgresql://localhost:5432/cashFlow
    DB_USER=your_username
    DB_PASSWORD=your_password
    JWT_SECRET=your_super_secret_key
    ```

3.  **Google OAuth2**: Update the Google Client ID and Secret in `application.properties` if you plan to use Google login.

### 🏃 Running the Application

Clone the repository and run:

```bash
./mvnw spring-boot:run
```

The server will start at `http://localhost:8080`.

---

## 📑 API Endpoints

### Authentication
- `POST /api/auth/register` - Create a new account.
- `POST /api/auth/login` - Log in and receive a JWT token.
- `GET /api/auth/me` - Get current user profile.

### Expenses
- `GET /api/expenses` - Get all expenses for the logged-in user.
- `POST /api/expenses` - Create a new expense.
- `DELETE /api/expenses/{id}` - Remove an expense by ID.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

## 📄 License

This project is licensed under the MIT License.

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/Harshvardhan210">Harshvardhan</a>
</p>
