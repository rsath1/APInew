

---

# ContosoPizza API

## Overview

The ContosoPizza API is a simple RESTful API built with ASP.NET Core. It provides endpoints to manage pizza entities, allowing clients to perform CRUD (Create, Read, Update, Delete) operations. This project demonstrates how to build and structure a basic API with ASP.NET Core.

## Project Structure

- **Models**: Contains the data models used by the API.
- **Services**: Includes the business logic and data access methods.
- **Controllers**: Defines the API endpoints and handles HTTP requests.

## API Endpoints

### 1. Get All Pizzas

- **Endpoint**: `GET /pizza`
- **Description**: Retrieves a list of all pizzas.
- **Response**: `200 OK` with a list of pizzas in JSON format.

### 2. Get Pizza by ID

- **Endpoint**: `GET /pizza/{id}`
- **Description**: Retrieves a specific pizza by its ID.
- **Parameters**:
  - `id` (int): The ID of the pizza to retrieve.
- **Response**:
  - `200 OK` with the pizza details in JSON format.
  - `404 Not Found` if the pizza with the given ID does not exist.

### 3. Create a New Pizza

- **Endpoint**: `POST /pizza`
- **Description**: Creates a new pizza.
- **Request Body**: JSON object representing the new pizza.
- **Response**:
  - `201 Created` with the created pizza details in JSON format.
  - `400 Bad Request` if the request is invalid.

### 4. Update an Existing Pizza

- **Endpoint**: `PUT /pizza/{id}`
- **Description**: Updates an existing pizza.
- **Parameters**:
  - `id` (int): The ID of the pizza to update.
- **Request Body**: JSON object representing the updated pizza.
- **Response**:
  - `200 OK` with the updated pizza details in JSON format.
  - `404 Not Found` if the pizza with the given ID does not exist.
  - `400 Bad Request` if the request is invalid.

### 5. Delete a Pizza

- **Endpoint**: `DELETE /pizza/{id}`
- **Description**: Deletes a specific pizza by its ID.
- **Parameters**:
  - `id` (int): The ID of the pizza to delete.
- **Response**:
  - `204 No Content` if the pizza was successfully deleted.
  - `404 Not Found` if the pizza with the given ID does not exist.

## Getting Started

1. **Clone the Repository**

    ```bash
    git clone https://github.com/your-username/ContosoPizza.git
    cd ContosoPizza
    ```

2. **Install Dependencies**

    ```bash
    dotnet restore
    ```

3. **Run the Application**

    ```bash
    dotnet run
    ```

4. **Access the API**

    Open your browser or API client (e.g., Postman) and navigate to `http://localhost:5000/pizza` to test the API endpoints.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request with your changes. 

## License

This project is licensed under the Apache license License - see the [LICENSE](LICENSE) file for details.

---

Feel free to adjust any details or add more specific instructions based on your project's requirements!
