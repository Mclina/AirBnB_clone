AirBnB_clone - The Console
Command interpreter to manage the AirBnB objects

About this project
The AirBnB_clone is the first step towards building our first full web application.
This web application is composed by:

A command interpreter to manipulate data without a visual interface, like in a Shell (perfect for development and debugging).
A website (the front-end) that shows the final product to everybody: static and dynamic
A database or files that store data (data = objects).
An API that provides a communication interface between the front-end and your data (retrieve, create, delete, update them).
console In this project, we will manipulate 2 types of storage: file and database.
In this repository, we will focus only on the command interpreter and file storage.
About the command interpreter (the console)
Command line interpreter that manipulates data and manages serialization and deserialization of objects.
How it works
The console:

Displays the prompt (default prompt: "(cmd)", our prompt: "(hbnb)") and waits for user input.
Reads the entered command and the argument.
Looks for the function of the command. For example: entering the command "all", makes the console looks for "do_all(self, arg)" function.
Executes the function.
If the typed command (the function) doesn't exist, the console prints an Error message.
Quits when the user enters "quit" or "EOF" or presses Ctrl+d.
Usage
Your shell should work like this in interactive mode:

$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$
But also in non-interactive mode: (like the Shell project in C)

$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
Project Structure
.
__AUTHORS
__console.py
__ models
__  __init__.py
__amenity.py
__base_model.py
 __city.py
__engine
__  __init__.py
 __file_storage.py
 __place.py
 __review.py
 __state.py
 __user.py
 __README.md
__tests
__  __init__.py
__ test_models
__    __init__.py
__engine
__  __init__.py
__test_file_storage.py
__test_amenity.py
__test_base_model.py
__test_city.py
__test_place.py
__test_review.py
__test_state.py
___test_user.py
Installation
You can run this program on your local machine by following these steps:

Step 1: Clone our repository using this command, (you need to have git and python3 installed on your machine first)

git clone https://github.com/Mclina/AirBnB_clone.git
Step 2: Change directory to AirBnB_clone:

cd AirBnB_clone
Step 3: Execute the console in this way:

./console.py

Step 4: enter your command (In this example, our command is "help")

(hbnb) help

Contributors
This project was written by Mariacelin Oshiomah. See the AUTHORS file for more information.
