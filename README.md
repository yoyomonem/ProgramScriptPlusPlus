# ProgramScript++
This is a simple interpreted programming language that has syntax and features heavily inspired by Python, JavaScript, and MATLAB. Basically NoodleScript, but more JavaScript-like.

# Syntax and Features
## Comments
```
# This is a comment
```
## Variables
```
var number = 10
var bool = true
var string = "Hello"
var list = [10 true "Hello"]
```
## Constant Variables
```
const var x = 10
x = 10  # Doesn't work
```
## IO
### print()
```
print("Hello World!\n")  # Outputs `Hello World!` to the console
```
### receive()
```
input = receive()  # Parses input from user as a string
```
### If Statements
```
if condition
  # Body
end
```
### Else Statements
```
if condition
  # Body
else
  # Body
end
```
### While Loops
```
while condition
  # Body
end
```
## Functions
```
def add(var num1 var num2)
  num1 + num2  # notice how no return statement is needed, like in Rust
end
```
## Nested Functions
```
def div(var num var den)
  def safeToDiv(var den)
      den != 0
  end

  if safeToDiv(den)
    num / den
  else
    print("Cannot divide by zero\n")
  end
end
```
## Built-In Functions
```
print()  # Outputs to console
printRaw()  # Outputs the runtime value of an expression
receive()  # Parses input as string
abs(num)  # Absolute value
floor(num)  # Rounds down value
round(num)  # Rounds value
ceil(num)  # Rounds value up
sqrt(num)  # Takes square root of value
pow(num num)  # Raises value to power
num(any)  # Converts value to a number
bool(any)  # Converts a value to a bool
str(any)  # Converts a value to a string
at(list num) # Accesses an element inside of a list
set(list num any)  # Sets an element in a list with a new value
append(list any)  # Adds an element to a list
pop(list num)  # Removes and returns an element from a list
```
# Anything Else?
Nope, just enjoy the debugging nightmare if you attempt to use this language. ;)
