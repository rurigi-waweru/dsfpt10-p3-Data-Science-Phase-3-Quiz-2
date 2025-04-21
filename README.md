# Quiz: Object-Oriented Programming



## Question 1:

Which of the following is the correct way to instantiate the `Driver` class?

```python
class Driver:
    def greeting(self):
	return "Hello, how are you today?"
```

(i) bill = Driver() 

(ii) bill.Driver() 

(iii) import Driver 

(iv) Driver.bill() 

(v) driver('bill')
The `correct` way to instantiate the Driver class is: `(i) bill = Driver()`



## Explanation:

(i) ✅ Correct: This is the standard syntax for creating an object (instance) of a class.

(ii) ❌ Incorrect: This would attempt to call a method named Driver on a variable bill, which is undefined.

(iii) ❌ Incorrect: import Driver is for importing a module, not instantiating a class.

(iv) ❌ Incorrect: This tries to call a method bill() on the class Driver, which doesn’t exist.

(v) ❌ Incorrect: driver('bill') implies driver is a callable (like a function or class), but it's undefined here, and Driver doesn’t take arguments in the constructor.



## Question 2:

When writing code, what statement can be used as a placeholder to prevent an indentation error?

(i) def

(ii) instance

(iii) class

(iv) pass

(v) break


The correct answer is: `(iv) pass`


## Explanation:

(iv) pass ✅ Correct: pass is a placeholder that does nothing but prevents an indentation error. It's often used in situations where code is required syntactically but you don’t want to implement it yet.

(i) def ❌ Incorrect: def is used to define a function, not to prevent indentation errors.

(ii) instance ❌ Incorrect: instance is not a keyword in Python and does not serve this purpose.

(iii) class ❌ Incorrect: class is used to define a class, not to handle indentation errors.

(v) break ❌ Incorrect: break is used to exit loops, not as a placeholder to prevent indentation errors.



## Question 3:

In the following example, what is the expected output?

```python 
class Bike:
	def color(self):
		return "The bike is Red"
	
	def style(self):
		return "The bike is a Road bike"

my_new_bike = Bike()
my_new_bike.style()
```

(i) AttributeError: 'Bike' object has no attribute 'style'


(ii) ’The bike is Red’


(iii) There is no output


(iv) <__main__.Bike object at 0x7fdf900313a0>


(v) ’The bike is a Road bike’


The correct answer is: `(v) 'The bike is a Road bike'`


## Explanation:

(v) 'The bike is a Road bike' ✅ Correct: The style() method is called on the my_new_bike object, which correctly returns "The bike is a Road bike".

(i) AttributeError ❌ Incorrect: There is no error because the style() method exists in the Bike class.

(ii) 'The bike is Red' ❌ Incorrect: The method color() is not called, so this output will not appear.

(iii) There is no output ❌ Incorrect: Calling my_new_bike.style() will indeed produce an output.

(iv) <__main__.Bike object at 0x7fdf900313a0> ❌ Incorrect: This output would happen if you tried to print the my_new_bike object itself without calling any methods.


## Question 4:

In the following example, which of the following outputs can you expect?

```python
class Cat:
	
	def meow():
		return "Meow, Purr!"

fifi = Cat()
fifi.meow()
```

(i) TypeError: meow() takes 0 positional arguments but 1 was given


(ii) ‘Meow, Purr!’


(iii) <bound method Cat.meow of <__main__.Cat object at 0x7fdf900313a0>>


(iv) AttributeError: 'Cat' object has no attribute 'meow'


(v) There is no output

The correct answer is: `(i) TypeError: meow() takes 0 positional arguments but 1 was given`

## Explanation:


(i) TypeError ✅ Correct: The method meow() is defined without a self parameter, which is required in instance methods. When calling fifi.meow(), Python automatically passes fifi as the first argument (i.e., self), causing the TypeError.

(ii) 'Meow, Purr!' ❌ Incorrect: The function would work if it had a self parameter, but it doesn’t, leading to an error.

(iii) <bound method Cat.meow of <__main__.Cat object at 0x7fdf900313a0>> ❌ Incorrect: This would happen if you accessed meow without calling it (e.g., fifi.meow), not when invoking it.

(iv) AttributeError: 'Cat' object has no attribute 'meow' ❌ Incorrect: The meow method exists; the issue is with the incorrect method definition.

(v) There is no output ❌ Incorrect: The error prevents any output from being generated.


## Question 5:


The creation of functions in programming languages made it easier to do which of the following?

(select all that apply)

(i) Break a program

(ii) Create a GOTO statement

(iii) Call a short script multiple times

(iv) Set global variables

(v) Reuse a subroutine



The correct answers are: 
```
(iii) Call a short script multiple times
(v) Reuse a subroutine
```

## Explanation:

(iii) Call a short script multiple times ✅ Correct: Functions allow you to define a block of code that can be called and executed multiple times, making the code more modular and reusable.

(v) Reuse a subroutine ✅ Correct: Functions are essentially reusable blocks of code (subroutines), which makes it easier to avoid repetition in your program.

(i) Break a program ❌ Incorrect: Functions themselves don't break a program; they help organize and structure code.

(ii) Create a GOTO statement ❌ Incorrect: Functions don’t create a GOTO statement, which is a separate control flow statement that is generally discouraged in modern programming due to its potential for creating spaghetti code.

(iv) Set global variables ❌ Incorrect: Functions can access or modify global variables, but they don't inherently make it easier to set them. In fact, the use of global variables can often complicate code.