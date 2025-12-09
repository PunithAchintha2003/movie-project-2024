# Movie Booking System

A Java web application for movie ticket booking and management built with Jakarta Servlets, JSP, and MySQL.

## Technology Stack

- **Java**: 11
- **Framework**: Jakarta Servlet API 5.0
- **Build Tool**: Maven
- **Database**: MySQL
- **Frontend**: JSP, Tailwind CSS
- **Payment**: Stripe

## Features

- User authentication and authorization
- Movie management (admin)
- Booking system
- Payment processing
- Review system
- Email verification

## Project Structure

```
src/main/
├── java/com/movieproject/
│   ├── controller/     # HTTP request handlers
│   ├── service/        # Business logic
│   ├── model/          # Domain entities
│   ├── utils/          # Utility classes
│   └── exception/      # Custom exceptions
├── resources/
│   └── config/         # Configuration files
└── webapp/
    ├── views/          # JSP pages
    ├── components/     # Reusable JSP components
    └── WEB-INF/        # Deployment descriptor
```

## Prerequisites

- Java 11 or higher
- Maven 3.6+
- MySQL 5.7+ or MariaDB
- Application server (Tomcat 9+, Jetty, etc.)

## Setup

1. Clone the repository
```bash
git clone <repository-url>
cd movie-project-2024/java-project
```

2. Configure database
   - Update `src/main/resources/config/db.properties` with your database credentials

3. Build the project
```bash
mvn clean install
```

4. Deploy to application server
   - Copy the generated WAR file from `target/` to your server's webapps directory
   - Or use your IDE's deployment feature

## Building

```bash
# Compile
mvn clean compile

# Run tests
mvn test

# Package WAR file
mvn clean package
```

The WAR file will be generated in the `target/` directory.

## Configuration

Database configuration is stored in `src/main/resources/config/db.properties`. Update the following properties:
- `db.url`: Database connection URL
- `db.username`: Database username
- `db.password`: Database password

## License

[Add your license here]
