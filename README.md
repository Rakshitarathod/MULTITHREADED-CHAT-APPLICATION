# MULTITHREADED-CHAT-APPLICATION

# Multithreaded Chat Application

## Overview
A Java-based real-time chat application that supports multiple clients with both broadcast and selective messaging capabilities. Built using Java Swing for the GUI and Java Sockets for networking.

## Features
- **Server-side:**
  - Handles multiple client connections
  - Username validation
  - Real-time user tracking
  - Message broadcasting
  - Selective messaging (multicast)
  - Disconnection notifications

- **Client-side:**
  - User registration
  - Message broadcasting
  - Selective messaging
  - Active user list
  - Clean disconnect

## Technical Details
- **Language:** Java
- **GUI:** Swing
- **Networking:** Java Sockets
- **Concurrency:** Multithreading
- **Data Structures:** ConcurrentHashMap, HashSet

## Installation & Usage

### Requirements
- Java JDK 8+


## ⚙️ How It Works

### 1. Server Side:
- `Server.java` starts a socket server on a fixed port.
- For each client connection, a new thread (`ClientHandler`) is created.
- Server broadcasts incoming messages to all connected clients.

### 2. Client Side:
- `Client.java` connects to the server using socket.
- Two threads are used:
  - One for sending user input to the server.
  - One for reading messages from the server.

---

## 🚀 How to Run
- ServerView.java - It contains code for server. This class must be run first.
- loginClient.java - It contains code for client's login and run after the server has been started. It can be run as many number of times depending upon number of clients required.
- ClientView.java - It contains code for the client.

1. **Start the Server**
   ```bash
   java server.Server
   ```

2. **Start Clients (in separate terminals)**
   ```bash
   java client.Client
   ```

3. Type messages and chat in real time!

---


## 🔒 Future Enhancements

- GUI using JavaFX or Swing
- Client-side username support
- Message encryption using AES
- Server command console for admin actions
- Logging chat history to a file

---

## Output
<img width="812" height="561" alt="Image" src="https://github.com/user-attachments/assets/31654ac0-0add-4a28-8dcf-1baf1d541f37" />
<img width="620" height="350" alt="Image" src="https://github.com/user-attachments/assets/8eb357ec-147a-4eb6-8cc3-76b47268a089" />
<img width="921" height="706" alt="Image" src="https://github.com/user-attachments/assets/a5f0591d-c048-4276-ba0d-0f629d67ba45" />
<img width="1725" height="741" alt="Image" src="https://github.com/user-attachments/assets/7bfe6273-3887-43ed-9932-68dbe6b118f8" />
