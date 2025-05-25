<h1 align="center">Todo API with Go</h1>

A lightweight RESTful API implemented in Go, providing CRUD operations for managing todo tasks.

## Features
- Create, Read, Update, and Delete (CRUD) todo tasks
- RESTful API design with clean endpoints
- JSON request and response format
- Error handling with appropriate HTTP status codes
- Built using Go and Gin for performance and simplicity


## Tech Stack
- Go standard library packages: `net/http`, `errors`
- [Gin-Gonic](https://github.com/gin-gonic/gin) web framework
- Postman (for API testing)


## Getting Started
Follow these steps to get a local copy of the project up and running:

### Prerequisites
- [Go](https://golang.org/dl/) installed (version 1.18 or higher recommended)
- Git installed
- (Optional) [Postman](https://www.postman.com/) or any API testing tool to test endpoints

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/msaakaash/todo-api-go.git
cd todo-api-go
```

2. **Initialize Go module**
If you have just cloned the repo and it doesn't contain a `go.mod` file, initialize the Go module by running:
```bash
go mod init todo-api-go
```

3. **Install dependencies**
Run the following command to download and install required packages, including Gin-Gonic:
```bash
go mod tidy
```

4. **Run the application**
Start the API server using:
```bash
go run main.go
```

5. **Test the API**
> **Note:** By default, the server runs on `http://localhost:9090`. Use Postman or curl to interact with the API.

### Example cURL request to get all todos
```bash
curl http://localhost:9090/todos
```
Feel free to customize and extend the API as needed!

## API Endpoints

| Method | Endpoint   | Description                  |
|--------|------------|------------------------------|
| GET    | /todos     | Retrieve all todo tasks      |
| GET    | /todos/:id | Retrieve a specific todo by ID |
| POST   | /todos     | Create a new todo            |
| PATCH  | /todos/:id | Update a todo by ID          |
| DELETE | /todos/:id | Delete a todo by ID          |

> **Note:** `PATCH` is typically used for partial updates to a resource. You may also use `PUT` when you want to fully replace or permanently update a resource.


## Contributing
Contributions are welcome! Please see [CONTRIBUTING.md](docs/CONTRIBUTING.md) for guidelines.

## Code of Conduct
Please read our [Code of Conduct](docs/CODE_OF_CONDUCT.md) before contributing to this project.

## Security
If you discover a vulnerability, please refer to our [Security Policy](docs/SECURITY.md) for instructions on how to report it responsibly.

## License  
This project is licensed under the [MIT License](LICENSE).


## Author

[**Aakaash M S**](https://github.com/msaakaash)
