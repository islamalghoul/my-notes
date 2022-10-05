[MainPage](../../../README.md)
# Part 1
## Unit tests and TDD?


Unit tests: are some pieces of code to exercise the input, the output and the behaviour of your code

TDD is ashort for Test-Driven Development 


### The Cycle
The cycle is made by three steps:

1-Write a unit test and make it fail

2- Write the feature and make the test pass

3- Refactor the code
# Part 2
## What does the if __name__ == “__main__”: do?
Before executing code, Python interpreter reads source file and define few special variables/global variables. 
If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable


### Advantages :
1-Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.

2-If you import this script as a module in another script, the __name__ is set to the name of the script/module.

3-Python files can act as either reusable modules, or as standalone programs.

4-if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.



# Part 3
## What is Recursion? 
The process in which a function calls itself directly or indirectly 

## Need of Recursion

Recursion is an amazing technique with the help of which we can reduce the length of our code and make it easier to read and write

[Refernce1](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)
[Refernce2](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)
[Refernce3](https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/)
