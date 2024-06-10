# Veterinary Management System

This project is developed as part of the capstone project for the Patika+ FullStack Web Developer Program. The project includes both backend and frontend components of a veterinary management system.

### Live Demo
You can experience this project live, which meets all requirements and has a user-friendly interface.
Access the live version of the project at [Live Demo](https://veterinarymanagementapp.netlify.app).
`Deployed with Render. It may open slowly on the first launch.`

- All CRUD, Search, and filter operations can be performed.
- Searches in Customer, Animal, Appointment, and Vaccine are done in the database, so you must write the `full names`.
- In Doctor and Report searches, you can search by writing `part of the names`.
- Appointments can only be made `on the hour`. For example, at 14:00, 15:00.
- You cannot add duplicate records. You will receive a `Conflict` error.

## Project Description

This project provides management for veterinarians, customers, and their animals. It also includes appointment and reporting features. The project includes the following features:

### Backend Development

- **Recording veterinarians**
- **Recording doctors' working days (available days)**
- **Recording customers**
- **Recording animals belonging to customers**
- **Creating appointments for animals with veterinarians**
- **Entering date and time while creating appointments**
- **Recording vaccinations applied to animals along with dates**
- **Creating reports and adding vaccinations to reports**

### Frontend Development

- **Login Page**
- **Customer Operations (CRUD)**
- **Veterinarian Operations (CRUD)**
- **Animal Operations (CRUD)**
- **Appointment Operations (CRUD)**
- **Vaccination Operations (CRUD)**
- **CRUD operations on each page**
- **User information (Modal)**
- **Design (CSS, Material)**

## Getting Started

To run your project locally, follow the steps below.

### Requirements

- Java 17+
- Node.js 14+
- PostgreSQL or MySQL
- Spring Boot
- React

### Setup

#### Backend

1. Clone the repository:
   ```sh
   git clone https://github.com/PehlivanMert/Veterinary-Api.git
   cd Veterinary-Api
   ```

2. Install dependencies and run the application:
   ```sh
   ./mvnw clean install
   ./mvnw spring-boot:run
   ```

3. Configure the database in the `application.properties` file.

4. Import the sample data using the `.sql` file:
   ```sh
   psql -U username -d database_name -f src/main/resources/data.sql
   ```
5. Alternatively, you can start the database and application using the `docker-compose up --build` command.
6. Once the application is running successfully, you can test the API at `http://localhost:8080` or `http://localhost:8080/swagger-ui/index.html#/`.

#### Frontend

1. Clone the repository:
   ```sh
   git clone https://github.com/pehlivanmert/vetapp-frontend.git
   cd vetapp-frontend
   ```

2. Install dependencies:
   ```sh
   npm install
   ```

3. Run the application:
   ```sh
   npm start
   ```

4. Once the application is running successfully, you can use it at `http://localhost:5173`.

## Usage

### Customer Operations

1. **Add Customer**: Enter and save customer information.
2. **Add Animal to Customer**: Select a customer, enter animal information, and save.
3. **Update and Delete Customer**: Update or delete customer information.

### Veterinarian Operations

1. **Add Doctor**: Enter and save doctor information.
2. **Add Doctor's Available Days**: Enter and save the doctor's available days.
3. **Update and Delete Doctor**: Update or delete doctor information.

### Appointment Operations

1. **Create Appointment**: Select animal and doctor, then create an appointment.
2. **Update and Delete Appointment**: Update or delete appointment information.

### Vaccination and Report Operations

1. **Create Report**: Create a report for an appointment.
2. **Add Vaccine to Report**: Add vaccination information to the report.

## UML Diagram

You can view the UML diagram of the project [here](img/VeterinaryUml.png).

## Contributing

1. Fork this repository.
2. Create a new feature branch: `git checkout -b feature/fooBar`
3. Commit your changes: `git commit -am 'Add some fooBar'`
4. Push to the branch: `git push origin feature/fooBar`
5. Submit a pull request.
6. Your pull request will be reviewed and merged.
7. After merging, you can delete your branch: `git branch -d feature/fooBar`
8. Thank you for contributing to the project!

## Contact

If you have any questions or feedback, please feel free to contact me:
- **Email**: [pehlivanmert@outlook.com.tr](mailto:pehlivanmert@outlook.com.tr)
- **GitHub**: [Mert Pehlivan GitHub](https://github.com/PehlivanMert)
