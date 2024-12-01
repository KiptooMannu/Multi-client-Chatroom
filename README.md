# Multi-client Chatroom
This Python-based multi-client chatroom application demonstrates the core concepts of socket programming and multi-threading in Python, enabling efficient communication among multiple clients.

Developed as part of the SPE 2404: Distributed & Network Programming assessment during the academic year 2024/2025 under the guidance of Dr. John Wainaina at Kirinyaga University, this project fulfills the course requirements by integrating client-server architecture, secure message handling, and fault tolerance mechanisms.

## Features
* Core
    * Multi-client
    * Admin authentication for server related activites
    * Full chatroom activity log
    * Individual user logs
    * User database w/ encrypted user passwords
    * Login system for returning users
* In-chat
    * Set or change preferred username
    * Set or change preferred password
    * Create, join or leave rooms
    * List users or rooms (admin only)
    * Send (encrypted) private messages

## Usage
1. Install dependencies
> pip3 install -r requirements.txt
2. Run server script
> python3 chat_server.py
3. Start server
    - Enter port number
    - Enter admin password
4. Run client script
> python3 chat_client.py [server_ip] [server_port]

## Client Options
```
/u [username]                       - Change the username
/p                                  - Change the password
/c [room_name]                      - Create a new room
/j [room_name]                      - Join a room
/l [room_name]                      - Leave a room
/cd [room_name]                     - Change default room
/list                               - (Admin) List all the rooms on the server
/users                              - (Admin) List all the users on the server
/public <[room_name]> [message]     - Sends a message to any room you are a part of
/private <[username]> [message]     - Send a (encrypted) private message to any user
/logout                             - Disconnect from the server
```
