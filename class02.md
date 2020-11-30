# TDD with Python
## Unit tests and TDD
Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.
But Test-Driven Development is a strategy to think (and write!) tests first.

* the structure

 convention widely used is the AAA: Arrange, Act and Assert
 - Arrange: you need to organize the data needed to execute that piece of code (input);
- Act: here you will execute the code being tested (exercise the behaviour);
- Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

* The Cycle
The cycle is made by three steps:
- 🆘Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)
- ✅ Write the feature and make the test pass! (you can dance after that)
- 🔵 Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)
> TDD is not about the money/tests

When we are writing tests we are forced to think about the design first and how we can break it into small pieces.
> A good library for tests is ```pytest```
# Recursion
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. 
### Why Stack Overflow error occurs in recursion? 
If the base case is not reached or not defined, then the stack overflow problem may arise
### direct and indirect recursion
A function fun is called direct recursive if it calls the same function fun. A function fun is called indirect recursive if it calls another function say fun_new and fun_new calls fun directly or indirectly
###  tailed and non-tailed recursion
A recursive function is tail recursive when recursive call is the last thing executed by the function
### How memory is allocated to different function calls in recursion?
When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to calling function and different copy of local variables is created for each function call. When the base case is reached, the function returns its value to the function by whom it is called and memory is de-allocated and the process continues.

