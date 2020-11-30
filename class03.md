## Reading and Writing Files in Python
### What Is a File?
a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

Files on most modern file systems are composed of three main parts:

1. Header: metadata about the contents of the file (file name, size, type, and so on)
2. Data: contents of the file as written by the creator or editor
3. End of file (EOF): special character that indicates the end of the file
## File Paths

Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
File Name: the actual name of the file
Extension: the end of the file path pre-pended with a period (.) used to indicate the file type
### Opening and Closing a File in Python
```file. open()```

-There are three different categories of file objects:
- Text files
- Buffered binary files
- Raw binary files
### Reading and Writing Opened Files
```.read():```
 
 to read 5 bytes of a line each time using the Python .readline()
 ```reader.readline(5)```
 ### Iterating Over Each Line in the File
 
 ```
 while line != '':  
  print(line, end='')
  line = reader.readline()
  ```
  
 ## Python Exceptions
 exception error. This type of error occurs whenever syntactically correct Python code results in an error. The last line of the message indicated what type of exception error you ran into.
 
### Raising an Exception
We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.
```
if x > 5:
 raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
 ```
### The AssertionError Exception
We ```assert``` that a certain condition is met. If this condition turns out to be ```True```, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError ```exception```.
### The try and except Block: Handling Exceptions
The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.
```
try:
    linux_interaction()
except:
    pass
```    

- raise allows you to throw an exception at any time.
- assert enables you to verify if a certain condition is met and throw an exception if it isn’t.
- In the try clause, all statements are executed until an exception is encountered.
- except is used to catch and handle the exception(s) that are encountered in the try clause.
- else lets you code sections that should run only when no exceptions are encountered in the try clause.
- finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.
