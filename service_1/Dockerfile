# Stage 1: Build the Go binary
FROM golang:1.22 AS builder

# Set the working directory inside the container
WORKDIR /app

# Copy go source code
COPY main.go .

# Build the Go binary
RUN go build -o service1 main.go

# Stage 2: Run the Go binary in a smaller image
FROM debian:bookworm-slim

# Set working directory
WORKDIR /app

# Copy the binary from the builder stage
COPY --from=builder /app/service1 .

# Expose the port the app runs on
EXPOSE 8001

# Command to run the binary
CMD ["./service1"]

