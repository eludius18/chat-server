# Rust Chat Server

This is a simple multi-user chat server written in Rust using the Tokio library. The server listens for incoming connections on localhost port 8080. When a client sends a message, the server broadcasts the message to all connected clients.

## Prerequisites

- Rust: You need to have Rust installed on your machine. You can download Rust from the [official website](https://www.rust-lang.org/tools/install).

## How to Run

Follow these steps to run the chat server:

1. **Start the server**: Open a terminal, navigate to the project directory, and run the following command:

    ```bash
    cargo run
    ```

    This command builds and runs the server. The server will start listening for incoming connections on localhost port 8080.

2. **Connect a client**: Open a new terminal window and run the following command:

    ```bash
    nc -v localhost 8080
    ```

    This command uses the `nc` (netcat) utility to connect to the server. You can open multiple terminal windows and run this command to simulate multiple clients.

3. **Send messages**: After connecting a client, you can type a message into the terminal and press Enter to send it. The server will broadcast the message to all connected clients.
