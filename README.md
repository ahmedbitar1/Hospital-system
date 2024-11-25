# Hospital Management System

## Overview
The **Hospital Management System** is a comprehensive solution featuring two projects:
1. **ASP.NET Web API**: A backend API providing endpoints for managing hospital operations.
2. **ASP.NET MVC Application**: A client application that consumes the API to provide a user-friendly interface for hospital staff and administrators.

This system is designed to streamline hospital operations such as patient management, staff scheduling, and appointment tracking. It includes robust authentication and authorization using **ASP.NET Identity** and **JWT**.

---

## Features

### API Project
- RESTful API endpoints for CRUD operations.
- Secure user authentication and authorization using JWT.
- Role-based access control (admin, doctor, staff, etc.).
- Data validation and error handling.

### MVC Project
- User-friendly interface for consuming the API.
- Features for patient, doctor, and staff management.
- Appointment scheduling and tracking.
- Real-time data fetched via API.

### Security Features
- User authentication and role-based authorization with **ASP.NET Identity**.
- Secure communication with **JWT (JSON Web Tokens)**.

---

## Technologies Used

### Backend (API)
- **Framework**: ASP.NET Web API
- **Authentication**: ASP.NET Identity, JWT
- **Language**: C#
- **Database**: SQL Server
- **Tools**: Entity Framework

### Frontend (MVC)
- **Framework**: ASP.NET MVC
- **Language**: C#
- **UI Framework**: Bootstrap
- **API Consumption**: HttpClient

---

## Getting Started

### Prerequisites
Before you begin, ensure you have met the following requirements:
- **Visual Studio 2022** or later.
- **.NET Framework** (minimum version specified in the project).
- **SQL Server** for database management.
- **Postman** or a similar API testing tool (optional, for testing API endpoints).

---

## Installation

### Step 1: Clone the Repository
Clone the repository to your local machine using the following command:

### Step 2: Set Up the API Project
1. Navigate to the **API project** folder inside the solution.
2. Open the `hospital.sln` solution file in **Visual Studio**.
3. Restore the required NuGet packages:
   - In **Visual Studio**, go to **Tools** > **NuGet Package Manager** > **Manage NuGet Packages for Solution** and restore any missing packages.
4. Update the database connection string in the `appsettings.json` file:
5. Apply migrations to create the database schema:
6. Build and run the API project to start the backend server.

### Step 3: Set Up the MVC Project
1. Navigate to the **MVC project** folder inside the solution.
2. Update the `appsettings.json` file to point to the local server where the API project is running:
3. Restore NuGet packages and build the project.
4. Run the MVC project to start the frontend application.

---

## Usage

### API Testing

1. **Test API Endpoints with Postman (Optional)**  
You can test the API endpoints using **Postman** or any other API testing tool.  
- Obtain a **JWT** token by sending a `POST` request to the login endpoint (`/api/auth/login`).
- Pass the JWT token in the **Authorization** header for subsequent requests to protected endpoints.

### MVC Application

1. **Access the Application**  
- Open a browser and go to `http://localhost:port-number` to access the MVC application.

2. **Login**  
- Use the credentials created during registration or from seed data to log in.

3. **Manage Hospital Operations**  
- You can now use the MVC interface to:
  - Manage patients.
  - Schedule appointments.
  - View patient records.
  - View and manage hospital staff.

---

## Project Structure

### API Project

- **Controllers**: Handles API requests and contains business logic.
- **Models**: Defines data structures and validation rules.
- **Services**: Implements core application logic for API operations.
- **Data**: Contains database context and migration configurations.

### MVC Project

- **Controllers**: Manages user interactions, handles API communication, and sends data to views.
- **Views**: Razor-based templates used to render UI components.
- **Models**: Defines view-specific data structures for API data.

---

## Authentication Workflow

1. **Registration**  
Users can register via the API, where their data is securely stored in the database.

2. **Login**  
Users log in to the system with their credentials and receive a **JWT** token.

3. **Token Usage**  
The JWT token is sent with each API request in the **Authorization header** for authentication.

4. **Role-Based Access Control**  
The API and MVC routes enforce role-based access, ensuring only authorized users can access certain data and features based on their roles (e.g., admin, doctor, staff).

---

## Contributing

We welcome contributions! Here’s how you can get started:

1. **Fork the Repository**  
Fork the repository to your GitHub account.

2. **Create a New Branch**  
Create a new branch for your feature or bugfix:

3. **Make Changes and Commit**  
Make your changes and commit them:

4. **Push to the Branch**  
Push your changes to the branch:

5. **Submit a Pull Request**  
Submit a pull request for review.

---

## License

This project is licensed under the **MIT License**.

---

## Contact

For any questions or support, feel free to reach out:
- **Name**: [Ahmed Esam Elbitar]
- **Email**: [ahmedesamo778@gmail.com]


