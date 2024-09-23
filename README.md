# News App

## Project Overview
The **News App** is a full-stack application that allows users to search, read, and save news articles to their favorites list. The application fetches news data using the [Newscatcher API](https://newscatcherapi.com/) and offers a responsive, user-friendly interface that runs smoothly on various devices. Users can register, log in, search for news, and manage their favorite articles.

## Objective
The objective of this project is to develop a scalable, responsive, and user-friendly news application with the following core features:
- Search for news articles
- Read news articles in HTML format
- Save articles to a favorites list
- Fetch news articles via API integration with Newscatcher API

## Features

### Functional Requirements
- **User Registration and Login**: Secure user registration and login with authentication.
- **Display News Articles**: List common news articles fetched from the API.
- **Search Functionality**: Search for specific news articles.
- **View News Article**: Open and read any article from the list.
- **Favorite Articles**: Add articles to a favorites list and view them.
- **Responsive UI**: The application should function well on various devices, from mobile phones to desktops.
- **User-Friendly UI**: The UI should be intuitive and visually appealing.

### Non-Functional Requirements
- **Performance**: Quick and smooth loading of news articles, even on low-end devices.
- **Scalability**: The app should support a large number of users without performance degradation.
- **Usability**: Easy navigation and operation for users, regardless of experience.
- **Security**: Protection of user data from unauthorized access, modification, or deletion.

## Technical Specifications

### Backend
- **Architecture**: Microservices
- **Authentication**: Secured with JWT tokens
- **API Gateway**: Manages API requests and routing
- **Service Discovery**: Ensures efficient service-to-service communication
- **Configuration Server**: Manages dynamic configuration for microservices

### Frontend
- **Framework**: Angular or React
- **Responsive Design**: Built with responsiveness to ensure compatibility with multiple device types

### Database
- **SQL Database**: Integrated with cloud-based SQL database for storing user data and favorites

### Deployment
- **Cloud Platform**: AWS for hosting and deployment
- **CI/CD**: Continuous Integration and Continuous Deployment setup on AWS

### Other Tools and Technologies
- **Source Control**: Gitlab for version control
- **API Documentation**: Swagger/Open API for documenting backend services
- **Testing**: Comprehensive unit and integration tests
- **Message Broker**: RabbitMQ or Kafka for handling asynchronous messaging between microservices
- **Containerization**: Docker and Docker Compose for containerizing services
- **Code Quality**: Tools integrated to ensure code quality
- **CI Tools**: Continuous integration using Gitlab CI/CD

## Tools and Technologies
| Category               | Technology                        |
|------------------------|------------------------------------|
| **SCM**                | Gitlab                             |
| **Frontend**           | Angular/React                      |
| **Backend**            | Microservices with Spring Boot     |
| **Database**           | SQL on Cloud                       |
| **Middleware**         | RabbitMQ/Kafka                     |
| **Containerization**   | Docker, Docker Compose             |
| **Cloud**              | AWS                                |
| **Testing**            | JUnit, Mockito                     |
| **Code Quality**       | SonarQube                          |
| **CI/CD**              | Gitlab CI/CD on AWS                |
| **API Documentation**  | Swagger                            |

## Setup and Installation

### Prerequisites
- Node.js (for frontend development)
- Java 8/11 (for backend development)
- Docker
- Gitlab account (for CI/CD and source control)

### Steps to Run Locally

1. **Clone the Repository**:
    ```bash
    git clone <repository-url>
    cd news-app
    ```

2. **Backend Setup**:
    - Navigate to the `backend` directory.
    - Install dependencies and run the application:
      ```bash
      mvn clean install
      mvn spring-boot:run
      ```

3. **Frontend Setup**:
    - Navigate to the `frontend` directory.
    - Install dependencies and run the app:
      ```bash
      npm install
      npm start
      ```

4. **Running with Docker**:
    - Ensure Docker is installed and running.
    - Build and run Docker containers:
      ```bash
      docker-compose up --build
      ```

## Testing

### Unit and Integration Testing
The application includes comprehensive unit tests and integration tests for both frontend and backend components. These tests can be run using the following commands:

- **Backend Tests**:
    ```bash
    mvn test
    ```

- **Frontend Tests**:
    ```bash
    npm test
    ```

## API Documentation
API documentation is provided using **Swagger**. After running the backend service, you can access the documentation at:

