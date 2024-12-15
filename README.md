# Spring Boot Project Template

This repository serves as a template for creating Spring Boot projects. It includes configurations and best practices to kickstart your development.

## Table of Contents
- [Features](#features)
- [Setup and Installation](#setup-and-installation)
- [Project Structure](#project-structure)
- [Environment Variables](#environment-variables)
- [Scripts](#scripts)
- [License](#license)

---

## Features
- Pre-configured `.env` support for managing environment variables.
- `.gitignore` tailored for Spring Boot projects.
- Maven build system.
- Ready-to-use database configurations.
- Clean and modular project structure.

---

## Setup and Installation

1. **Clone the repository**
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. **Set up the environment variables**
   Create a `.env` file in the root directory and configure it as needed:
   ```env
   # Example .env file
   SERVER_PORT=8080
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_NAME=my_database
   DB_USERNAME=root
   DB_PASSWORD=password123
   ```

3. **Build the project**
   ```bash
   ./mvnw clean install
   ```

4. **Run the application**
   ```bash
   ./mvnw spring-boot:run
   ```

---

## Project Structure
```
src/
├── main/
│   ├── java/       # Application source code
│   ├── resources/  # Application resources (e.g., application.yml)
│   │   ├── static/   # Static web assets
│   │   └── templates/ # Template files for Thymeleaf (if used)
│
├── test/           # Test files
```

---

## Environment Variables
Use a `.env` file to define environment-specific variables such as database credentials and server configurations. The project uses `spring-dotenv` to load variables from `.env` automatically.

Example:
```env
DB_HOST=127.0.0.1
DB_PORT=3306
DB_NAME=my_database
DB_USERNAME=root
DB_PASSWORD=password
```

---

## Scripts
### Maven Commands
- **Build the application:**
  ```bash
  ./mvnw clean install
  ```
- **Run the application:**
  ```bash
  ./mvnw spring-boot:run
  ```
- **Run tests:**
  ```bash
  ./mvnw test
  ```

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
