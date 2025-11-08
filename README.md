# Network File Sharing – Server and Client

## Project Overview
This project implements a **TCP-based file transfer system** using **C++**.
It includes both a **server** and **client** application that communicate over sockets to transfer text files.

The server listens for incoming connections, receives data from the client, and saves it into a file.
The client connects to the server, sends data, and logs the transfer process.

---

## Project Structure
```
Network_File_Sharing_Server_And_Client/
├── Data/
│ ├── Client/
│ │ └── client_text.txt
│ └── Server/
│ └── server_text.txt
├── include/
│ ├── client.h
│ ├── logging.h
│ └── server.h
├── src/
│ ├── client.cpp
│ └── server.cpp
├── .gitignore
├── README.md
└── Makefile (optional if created)
```
---

---

## Files Description
| File / Folder | Description |
|----------------|-------------|
| `src/server.cpp` | Contains server-side implementation for handling socket creation, binding, listening, and receiving file data. |
| `src/client.cpp` | Contains client-side implementation for creating a connection to the server and transmitting data. |
| `include/server.h` | Header file for server declarations. |
| `include/client.h` | Header file for client declarations. |
| `include/logging.h` | Header file providing a simple logger utility for info/debug/error messages. |
| `Data/Server/Server_Final_Text.txt` | Output file where the server writes received data. |
| `Data/Client/Client_Final_Text.txt` | Input/output file used by the client during file transfer. |

---

## Compilation and Execution

### 1. Compilation
Run the following commands to compile the source files and create the executables. Ensure you use the **`std=c++20`** flag to support modern C++ features.

```bash
g++ -o server src/server.cpp -Iinclude -std=c++20
g++ -o client src/client.cpp -Iinclude -std=c++20
chmod +x server

./server
./client
```
---

✅ **Instructions:**
1. Open your project in VS Code.
2. Open `README.md`.
3. Delete any old text and **paste everything above**.
4. Save (`Ctrl + S`).
5. Push to GitHub

