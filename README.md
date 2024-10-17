# Config Repository

This project is a configuration server for the microservices of the employee management application. It uses Spring Cloud Config to manage and centralize the configuration for various services, including `department-service`, `employee-service`, `user-service` and `auth-service`.

## Project Structure

```
config-repository/
├── .gitignore
├── README.md
├── auth-service.properties
├── department-service.properties
├── employee-service.properties
├── user-service.properties
```

## Requirements

- Java 11 or higher
- Maven

## Configuration

The configuration server is set up to read properties from specific files for each service. The configuration files are located in the `src/main/resources` directory.

### Example Configuration Files

- `department-service.properties`
- `employee-service.properties`
- `user-service.properties`

Each configuration file contains properties specific to its respective service.

## Running the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/solomon-java-angular-playground/employee-management-system
   cd Backend/config server/src/main/java/com/teleconsys/config_server/
   ```

2. Run the project with Maven:

   ```bash
   mvn spring-boot:run
   ```

## Usage

Once started, the configuration server will be accessible at `http://localhost:9075`. You can use the Spring Cloud Config APIs to retrieve configurations for the services.

## Services ports

- department-service: 9080
- employee-service: 9085
- user-service: 9090

## Contributing

If you would like to contribute, please open an issue or create a pull request.

## License

This project is licensed under the MIT License.
