# What is C#?
### C# (pronounced "C Sharp") is a programming language developed by Microsoft.
### C# is a type-safe object-oriented programming language.
### C# is a simple, modern, general-purpose, object-Oriented programming language developed by Microsoft within its .NET initiative.

### C# is designed for CLI(Common language Infrastructure), which consists of the executable code and runtime environment that allows us of various high-level languages on different computer platforms and architectures. Few things makes C# widely used languages:
1. **modern, general-purpose programming language.**
2. **Object Oriented, component Oriented, structured languages.**
3. **Is also a part if .NET Framework.**

---

# Good to know Information
---
### What is different between Statically typed and Dynamically typed programming?

#### Statically typed programming languages do type checking (the process of verifying and enforcing the constraints of types) at compile-time as opposed to run-time. Statically typed languages binds the type to a variable for its entire scope.

#### Dynamically typed programming languages do type checking at run-time as opposed to Compile-time. It is not typed safe. Can be more flexible  by allowing programs to generate types and functionality based on run-time data), though at the expense of fewer a priori guarantees. Dynamic typing may result in runtime type errors—that is, at runtime, a value may have an unexpected type, and an operation nonsensical for that type is applied. Fewer complier time. Dynamically typed languages bind the type to the actual value referenced by a variable.
---

# What is CLR?
### It is the execution engine of .NET Framework where all the .NET Applications runs under supervision of CLR.
1. Applications which run under the CLR are provided with certain features like:
    * Security
    * Portability
    * Automatic memory management.
  ### CLR internally contains the following things in it:
    * Security Manager
    * JIT Compiler
    * Garbage Collector
---

# What is Object?
### An object is a concrete entity based on a class, and is sometimes referred to as an instance of a class.
* "New" keyword is used to create an object.
* It is a real time object.
 ---

# What is the difference between a struct and a class in C#?
### Class and struct both are the user defined data type but have some major difference:

1. Struct
    * The struct is value type in C# and it inherits from System.Value Type.
    * Struct is usually used for smaller amounts of data.
    * Struct can’t be inherited to other type.
    * A structure can't be abstract.
    * No need to create object by new keyword.
    * Do not have permission to create any default constructor.

2. Class

  * The class is reference type in C# and it inherits from the System.Object Type.
  * Classes are usually used for large amounts of data.
  * Classes can be inherited to other class.
  * A class can be abstract type.
  * We can’t use an object of a class with using new keyword.
  * We can create a default constructor.

---
#  What is the difference between Interface and Abstract Class?
###
---

# What is the difference between “continue” and “break” statements in C#?
### Using break statement, you can 'jump out of a loop' whereas by using continue statement, you can 'jump over one iteration' and then resume your loop execution.

---
# What is the difference between constant and read only in c#?
### Constant (const) and Readonly (readonly) both looks like same as per the uses but they have some differences:

### Constant is known as “const” keyword in C# which is also known immutable values which are known at compile time and do not change their values at run time like in any function or constructor for the life of application till the application is running.

### Readonly is known as “readonly” keyword in C# which is also known immutable values and are known at compile and run time and do not change their values at run time like in any function for the life of application till the application is running. You can assay their value by constructor when we call constructor with “new” keyword.
# is a subset of type casting.

---

# Define Property in C#.net?
### Properties are members that provide a flexible mechanism to read, write or compute the values of private fields.

---

# What is extension method in c# and how to use them?
### Extension methods enable you to add methods to existing types without creating a new derived type, recompiling, or otherwise modifying the original type.

---
# What is the difference between dispose and finalize methods in c#?
###
---

#  What is the difference between “out” and “ref” parameters in C#?
### “out” parameter can be passed to a method and it need not be initialized where as “ref” parameter has to be initialized before it is used.

---






[Next Lesson 1: Variables](./Lesson-1.md)
