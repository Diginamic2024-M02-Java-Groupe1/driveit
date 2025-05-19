# DriveIt

## 🚗 Transportation Management System

DriveIt is a comprehensive transportation management system developed as part of the Diginamic "Projet Fil Rouge" initiative. The application provides an integrated solution for managing transportation services.

## 🛠️ Tech Stack

### Backend
- Java with Spring Boot
- Maven for dependency management
- MariaDB database
- RESTful API with Swagger documentation

### Frontend
- Angular framework
- TypeScript/JavaScript
- NPM for package management

### DevOps
- Docker for containerization
- Docker Compose for multi-container orchestration

## 🏗️ Architecture

The application follows a microservices architecture with:
- **Database Layer**: MariaDB for data persistence
- **API Layer**: Spring Boot application exposing RESTful endpoints
- **Frontend Layer**: Angular application for the user interface
- **DevOps**: Containerized deployment with Docker

## 🚀 Setup and Installation

### Prerequisites
- Docker and Docker Compose
- Java 11+ (for local development)
- Node.js and NPM (for local development)

### Environment Configuration
1. Create a `.env` file in the project root based on the provided `.env.template`:
   ```bash
   cp .env.template .env
    ```
2. Create a `secret.properties` file in `api/src/main/resources/` for mail configuration:
    ```properties
   spring.mail.username=your_email@gmail.com
   spring.mail.password=your_app_password
   ```
   
### Running the Application
```bash
docker compose up
```

## 💻 Development

### API Development
The API is automatically rebuilt when changes are detected in the `./api` directory.

### Frontend Development
The Angular app is automatically rebuilt when changes are detected in the `./app` directory.

### Database Access
Access the database through PHPMyAdmin at `http://localhost:8081`

## 📚 Documentation
- API documentation available at `http://localhost:8080/swagger-ui`

## 🔒 Security Notes
- Sensitive configuration is stored in `.env` and `secret.properties` files (not tracked by Git)
- Database credentials should be changed in production environments

## 👥 Contributing
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License
[MIT License](LICENSE)
