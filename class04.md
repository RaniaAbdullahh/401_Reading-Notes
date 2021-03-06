## Classes and Objects

Objects are an encapsulation of variables and functions into a single entity.
Objects get their variables and functions from classes. Classes are essentially a template to create your objects.
ex:
```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()
myobjecty = MyClass()

myobjecty.variable = "yackity"

# Then print out both values
print(myobjectx.variable)
print(myobjecty.variable)
```

## Recursive Functions in Python
 recursive function is a function defined in terms of itself via self-referential expressions.

This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result.
All recursive functions share a common structure made up of two parts: base case and recursive case.
### Maintaining State

When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

- Thread the state through each recursive call so that the current state is part of the current call’s execution context
- Keep the state in global scope

###Recursive Data Structures in Python
A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure

## Naive Recursion is Naive
The Fibonacci numbers were originally deﬁned by the Italian mathematician Fibonacci in the thirteenth century to model the growth of rabbit populations. Fibonacci surmised that the number of pairs of rabbits born in a given year is equal to the number of pairs of rabbits born in each of the two previous years,
starting from one pair of rabbits in the ﬁrst year.
