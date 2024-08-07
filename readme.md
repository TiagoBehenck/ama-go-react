# API with GO 

This repository contains a simple API with GO. 

## Getting started

### Prerequisites

- PostgreSQL
- Docker

### Running the application

1. Create a database
2. Run the migrations
3. Run the application

Create `.env` file with the following content
```
WSRS_DATABASE_PORT=
WSRS_DATABASE_USER=
WSRS_DATABASE_PASSWORD=
WSRS_DATABASE_NAME=
WSRS_DATABASE_HOST=
```

```bash
# Run the application
docker compose up -d
go generate ./...
go run cmd/wsrs/main.go
```
