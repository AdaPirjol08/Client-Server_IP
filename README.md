# Socket Command Server

A simple server application demonstrating socket programming in C. This project processes commands sent by a client and performs predefined actions for each command.

## Features

- **Socket Communication**: Handles connections and communication with clients.
- **Command Parsing**: Processes client-sent commands and performs specific actions.
- **Command Responses**: Sends appropriate responses to the client for recognized and unrecognized commands.
- **Graceful Shutdown**: Allows the server to be stopped using a predefined command.

## Commands

- **`07#`**: Executes a specific action and responds with `"Command implemented"`.
- **`exit#`**: Closes the client connection and gracefully shuts down the server.
- **Unrecognized Commands**: Responds with `"Command not implemented"`.

## How It Works

1. Waits for a client connection.
2. Receives a command and processes it.
3. Executes predefined logic for recognized commands.
4. Closes the connection after processing each command.
5. Stops the server upon receiving the `exit#` command.

## Usage

1. **Compile the Program**:
   gcc -o server server.c

2. **Run the Server**:
   ./server

3. **Connect Using a Client** (e.g., telnet):
   telnet localhost 22037


## Learning Outcomes

- Hands-on experience with C socket programming.
- Understanding of client-server communication.
- Implementation of string parsing and command handling in C.

This project is ideal for showcasing foundational skills in systems programming and network communication.
