# ADV-Networking-Lab-Project
CSE348.2

Project Report: Basic Chat App (Message Board) using Sockets in Python

Introduction

The Basic Chat App, also referred to as a Message Board, is a Python project showcasing the fundamentals of socket programming to create a simple yet effective message board application. The primary objective is to establish real-time communication between a server and multiple clients over a network, allowing users to post and view messages.
Technologies Used

Python: The core programming language.
Sockets: Employed for network communication.
Select Module: Facilitates handling multiple connections efficiently.
Errno Module: Utilized for handling specific error codes related to non-blocking socket operations.
Visual Studio Code (VS Code): Used for coding and running the project.
Project Structure and Python Files

Server Side (server.py):     server_py.ipynb

Server Socket Creation:
Utilized the socket module to create a server socket.
Set socket options, including SO_REUSEADDR for reusing the address.

Connection Handling:
Used the select module to manage multiple client connections concurrently.
Implemented a function to receive messages from clients.

Client Management:
Maintained a list of connected clients.
Assigned a unique username to each client upon connection.

Message Broadcasting:
Broadcasted messages from one client to all connected clients.

Client Side (client.py):     client_py.ipynb

Client Socket Creation:
Created a client socket to connect to the server.
Set the socket to non-blocking mode.

User Interaction:
Captured the user's username for identification.
Enabled the user to post messages to the message board.

Message Handling:
Implemented a loop to receive and display messages from other clients.
Communication Protocol
Header Mechanism:
Utilized a header to prefix messages with their length.
Ensured proper encoding and decoding of messages to/from bytes.


Exception Handling:
Employed try-except blocks to handle non-blocking sockets gracefully.
User Interface
Console Interface:
Created a console-based interface for both the server and clients.
Enabled users to post messages and view the conversation.

Message Board Dynamics:
Emphasized the application's nature as a message board, where users can contribute to a shared space.
Challenges Faced
Non-Blocking Sockets:
Dealt with challenges related to non-blocking sockets and exceptions.
Ensured smooth communication without blocking the application.

Message Encoding/Decoding:
Ensured accurate encoding and decoding of messages to prevent data corruption.
Screenshots
In the screenshot, the Python-based Multi-Client Chat Application is showcased within Visual Studio Code. Users 'Rajin,' 'Zunayed,' 'Rakib,' and 'Ferdeus' actively engage in real-time conversations on the Message Board. The server efficiently manages concurrent connections, providing a practical demonstration of socket programming principles.

Future Improvements
Error Handling:
Implement more robust error handling for unexpected user actions.

Security Features:
Explore the addition of security features, such as message encryption.

Graphical User Interface (GUI):
Consider developing a GUI for a more user-friendly experience.
Conclusion
In conclusion, the Basic Chat App project, also serving as a Message Board, successfully demonstrates the implementation of a real-time communication platform using Python sockets. The project lays the foundation for further enhancements, such as improved error handling, security features, and a graphical user interface.
