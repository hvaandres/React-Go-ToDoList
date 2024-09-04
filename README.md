# React-Go-ToDoList
This project is both exciting and educational as I'm new to coding with Go. The goal is to develop a todo list application, structured across three branches:

Main Branch: Contains the core Go code for the basic todo list functionality.
Dev Branch: Integrates MongoDB for persistent storage of todos, ensuring data is saved in a database.
PRD Branch: Features a complete application with a React frontend and a Go backend, providing a graphical user interface for a more interactive experience.

# How to Install Go
- Download Go:

Visit the [Go Downloads page](https://go.dev/dl/) and download the installer for your operating system.

- Install Go:

Windows: Run the installer and follow the prompts.
macOS: Open the .pkg file and follow the instructions.
Linux: Extract the archive to /usr/local, and add the Go binary to your PATH.

```
tar -C /usr/local -xzf go1.x.x.linux-amd64.tar.gz
export PATH=$PATH:/usr/local/go/bin
```

- Verify Installation:

Open a terminal and run:
```
go version
```
You should see the installed Go version.


# How to Create a Database with MongoDB
- Install MongoDB:

Windows/macOS: Download the installer from the MongoDB Download Center and follow the installation instructions.
Linux: Use package managers or follow instructions from the MongoDB documentation.
Start MongoDB:

Windows/macOS: Run MongoDB as a service or use the mongod command.
Linux: Start MongoDB with the following command:

```
sudo systemctl start mongod
```

- Access MongoDB:

Open a terminal and run:
```
mongo
```
This will open the MongoDB shell where you can interact with your databases.

- Create a Database:

In the MongoDB shell, run:
```
use mydatabase
```
Replace mydatabase with your desired database name. This command switches to the specified database and creates it if it doesn’t already exist.

- Create a Collection:

Run the following command in the MongoDB shell to create a collection:
```
db.createCollection("mycollection")
```
Replace mycollection with your desired collection name.

# How to Initialize a Project with Go
- Create a New Directory:
```
mkdir myproject
cd myproject
```
- Initialize Go Module:

```
go mod init myproject
```
Replace myproject with your module name. This creates a go.mod file in your project directory.

- Create Your First Go File:

```
package main

import "fmt"

func main() {
    fmt.Println("Hello, Go!")
}

```
- Run Your Go Application:
```
go run main.go
```
You should see Hello, Go! printed in the terminal.
Add Dependencies (if needed):
```
go get <package-name>
```

This will update your go.mod and go.sum files with the new dependencies.
By following these steps, you’ll have Go installed, a MongoDB database set up, and a basic Go project initialized.
