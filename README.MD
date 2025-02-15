# grpc-java-sample

grpc-java-sample is a repository demonstrating a basic implementation of gRPC services and clients in Java.

---

## Overview

This project provides simple examples of how to build and run gRPC servers using Protocol Buffers. It is intended as a starting point for developers looking to integrate gRPC in their Java applications.

---
## Prerequisites

- **Java JDK 8+**
- **Maven** (or your preferred build tool)
- **Protocol Buffers Compiler (protoc)**  
  [Download and installation instructions](https://developers.google.com/protocol-buffers)

---
## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/grpc-java-sample.git
   cd grpc-java-sample
2. **Build the project:**
    ```bash
    mvn clean install

---
## Project Structure
grpc/
├── pom.xml                # Maven configuration file
├── src
│   └── main
│       ├── java         # Java source files
│       ├── resources    # Resources (e.g., configuration files)
│       └── resources   oto            # Protocol Buffers (.proto files)
└── README.md            # This file

---
## Testing with Postman using gRPC

Postman now supports gRPC requests, allowing you to test your gRPC services directly from the tool. To test the `Greeter/SayHello` method, follow these steps:

1. **Open Postman:** Launch the Postman application.
2. **Create a gRPC Request:** Click on "New" and select "gRPC Request".
3. **Set the URL:** In the request URL field, enter:
grpc://localhost:9090
4. **Import the Proto File (if needed):** Click on the "Import" button and load your `.proto` file to help Postman recognize the service and its methods.
5. **Select the Method:** From the list of available methods, choose `Greeter/SayHello`.
6. **Send the Request:** Click the "Invoke" button to send the gRPC request.
7. **Review the Response:** Check the response section in Postman to see the result of your call.
