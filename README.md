# AirBnB Clone - The Console

## Description

This project is a clone of the AirBnB console. It is a command-line interpreter that allows users to manage objects such as users, places, states, cities, amenities, and reviews. The console provides functionalities to create, read, update, and delete objects, and it uses a file storage system to persist the data.

## Command Interpreter

The command interpreter allows you to interact with the application via a command-line interface.

### How to Start It

To start the console, run the following command from the root directory of the repository:

### How to Use It

Once the console is started, you can use the following commands to manage your objects:

- `create <ClassName>`: Creates a new instance of the specified class and prints its id.
- `show <ClassName> <id>`: Prints the string representation of an instance based on the class name and id.
- `destroy <ClassName> <id>`: Deletes an instance based on the class name and id.
- `all [<ClassName>]`: Prints all string representations of all instances, or all instances of a specific class if provided.
- `update <ClassName> <id> <attribute name> "<attribute value>"`: Updates an instance based on the class name and id by adding or updating an attribute.

### Examples

```sh
$ ./console.py
(hbnb) create User
d4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8
(hbnb) show User d4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8
[User] (d4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8) {'id': 'd4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8', 'created_at': '2024-05-19T12:34:56.789012', 'updated_at': '2024-05-19T12:34:56.789012'}
(hbnb) all User
["[User] (d4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8) {'id': 'd4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8', 'created_at': '2024-05-19T12:34:56.789012', 'updated_at': '2024-05-19T12:34:56.789012'}"]
(hbnb) update User d4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8 name "John Doe"
(hbnb) show User d4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8
[User] (d4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8) {'id': 'd4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8', 'created_at': '2024-05-19T12:34:56.789012', 'updated_at': '2024-05-19T12:35:56.789012', 'name': 'John Doe'}
(hbnb) destroy User d4e1f6fc-1c34-4a7e-a5f5-7e3e8e69b5d8
(hbnb) all User
[]
(hbnb) quit

