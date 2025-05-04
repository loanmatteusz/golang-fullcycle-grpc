
# Go gRPC API - Category Service

This project implements a simple gRPC API for managing categories, built with Go. It supports basic CRUD operations and uses SQLite for storing category data.

## Features

- Create categories
- List all categories
- Retrieve a category by its ID
- Built with Go and gRPC
- SQLite for data storage

## Technologies

- **Go**: The primary programming language for the service.
- **gRPC**: High-performance, language-agnostic RPC framework.
- **SQLite**: Lightweight relational database for category storage.
- **Protocol Buffers (Proto3)**: For defining service contracts.

## Getting Started

### Requirements

- Go 1.20+
- SQLite3

### Generate Protocol Files

Before running the service, you need to generate Go files from the `category.proto` file. Run the following command:

```bash
protoc --go_out=. --go-grpc_out=. proto/course_category.proto
```

This will generate the required Go files for gRPC.

### Install Dependencies

To install the necessary dependencies for the project, run:

```bash
go mod tidy
```

### Run the Application

To start the gRPC server, use the following command:

```bash
go run cmd/grpc-server/main.go
```

This will start the server on port `50051`.


## License

This project is for educational purposes and part of the FullCycle 3.0 course.