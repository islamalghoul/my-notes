[MainPage](../../../README.md)


# What Is a File?

a file is a contiguous set of bytes used to store data

### Files on most modern file systems are composed of three main parts:
Header: metadata about the contents of the file (file name, size, type, and so on)
Data: contents of the file as written by the creator or editor
End of file (EOF): special character that indicates the end of the file

## Character Encodings
An encoding is a translation from byte data to human readable characters

## Opening and Closing a File in Python

the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object

## Reading and Writing Opened Files
Once you’ve opened up a file, you’ll want to read or write to the file. First off, let’s cover reading a file. There are multiple methods that can be called on a file object to help you out

## Working With Bytes
you may need to work with files using byte strings. This is done by adding the 'b' character to the mode argument

## Appending to a File
you may want to append to a file or start writing at the end of an already populated file. This is easily done by using the 'a' character for the mode argument

# Exceptions versus Syntax Errors
Syntax errors occur when the parser detects an incorrect statement
## The AssertionError Exception
you can also start by making an assertion in Python. We assert that a certain condition is met

## The try and except Block: Handling Exceptions

The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause
