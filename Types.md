## Reference Types
---
### Is set by storing the actual data (object) in memory and storing a reference to the object within the variable. Reference types in C# automatically support being set null.
---
## String
### A String is a sequence of zero or more unicode characters, surrounded by double quotes.

```
var myFirstName = "Subash";
var myLastName = "karki";

var fullName = myFirstName + myLastName; //Subash Karki

```
### split method
```
string aString = "1,2,3"; // the string to split
char[] separator = ",".ToCharArray(); // "," converted into an array of characters

// This splits `aString` using an array of separator `char` values
string[] numbers = aString.Split(separator); // numbers equals { "1", "2", "3" };

```
---

## Array

### Arrays allow you to combine multiple variables of the same type in a single variable. You declare an array type by specifying the type, followed by double square brackets type[].

### Arrays are zero-based index, meaning that the first value is stored at index 0. You can access a value using its index, along with square bracket notation.

```
var intsLiteral = new [] { 7, 58, 5 };

int firstNumber = intsLiteral[0]; // Equals 7
int secondNumber = intsLiteral[1]; // Equals 58

intsLiteral[2] = 10; // Did change 5 to 10

```
### join an array of strings into a single strings

```
string[] numbers = new [] { "1", "2", "3" }; // the array to join
string allNums = string.Join(",", numbers); // allNums equals "1,2,3"

```
---

## Reference vs. Value Types

###  **Value Type** :
#### A Value Type stores its contents in memory allocated on the _stack_. When you created a Value Type, a single space in memory is allocated to store the value and that variable directly holds a value. If you assign it to another variable, the value is copied directly and both variables work independently. Predefined datatypes, structures, enums are also value types, and work in the same way. Value types can be created at compile time and Stored in stack memory, because of this, Garbage collector can't access the stack.



### **Reference Type**:
#### Reference Types are used by a reference which holds a reference (address) to the object but not the object itself. Because reference types represent the address of the variable rather than the data itself, assigning a reference variable to another doesn't copy the data. Instead it creates a second copy of the reference, which refers to the same location of the heap as the original value. Reference Type variables are stored in a different area of memory called the _heap_. This means that when a reference type variable is no longer used, it can be marked for garbage collection. Examples of reference types are Classes, Objects, Arrays, Indexers, Interfaces etc.

---
## Stack vs Heap
### _Stack is used for static memory allocation and Heap for dynamic memory allocation, both stored in the computer's RAM ._


[Home](./README.md)                               [[Next Lesson 3: Methods](./Methods.md)
