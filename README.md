# usercount

A simple Go CLI tool that connects to a PostgreSQL database and returns the count of users.

## Requirements

- Go 1.25+
- PostgreSQL database

## Installation

```bash
go build -o usercount .
```

## Usage

Set the `DATABASE_URL` environment variable and run the tool:

```bash
DATABASE_URL="postgres://user:password@localhost:5432/dbname" ./usercount
```

The tool will output the number of users in the `public.users` table.

## Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `DATABASE_URL` | PostgreSQL connection string | Yes |
