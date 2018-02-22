##  C# Variables
---
### “Variables” are simply storage locations for data. You can place data into them and retrieve their contents as part of a C# expression. The interpretation of the data in a variable is controlled through “Types”.


### C# is strongly, and  statically-typed language meaning every variable has a type at compile time, and once type is set it cannot change, but its value can be changed.
###C# also allows **explicit** typing of any variable.
```
int myInt = 1;
float myFloat = 1f;
bool myBoolean = true;
string myName = "John";
char myChar = 'a';
double myDouble = 1.75;

```

### Type Inference is where you don't have to always explicit specify a type, let complier try to understand the type if variable automatically.

###The keyword _var_ is used to infer the type at compile time.

```
var name = "Subash Karki"; // compile as String.
name = "Sunil Karki"; //variable value can be changed but not the type

```

## C# Types
___
## Value Types:
#### It is set based on the provided value.
___

### Boolean ---> keyword == _bool_
#### Boolean type can only set value to be **true** or **false**.
```
bool isName = true;
isName = false;

```
---
### Character ---> keyword == _char_
#### You can set the value to any unicode character, surrounded by single quotes:
```
char myName = 's';

```
---
### Integer ----> keyword == int
#### You can set the value to be any integer between -2,147,483,648 to 2,147,483,647:
```
int myNumber = 29;
myNumber = -192;

```
---

### Decimal ----> keyword == Decimal
### you can set the value to be any decimal within the range of (-7.9 x 1028 to 7.9 x 1028) / 100 to 28 and appended with an m;
```
decimal myDecimal = 1234567890.234m;
myDecimal = -1234567890.234m;

```
----
### Enum ----> keyword == enum
#### Best to use when you want to limit the value set to a fixed amount of options.
```
using System;

class Enumerations
{
    enum Days
    {
        Monday,
        Tuesday,
        Wednesday,
        Thursday,
        Friday,
        Saturday,
        Sunday
    }

    static void Main()
    {
        Days day = Days.Monday;

        if (day == Days.Monday)
        {
            Console.WriteLine("It is Monday");
        }

        Console.WriteLine(day);

        foreach(int i in Enum.GetValues(typeof(Days)))
            Console.WriteLine(i);
    }
}

```

---
### Null and Nullables ---> syntax == ?
#### null == absence of value. null represents the absence of value: nothing is stored in memory or to disk.
```
bool? isBoolean = true;
		isBoolean = null;

		int? myInteger = null;
		myInteger = 0;

		string myString = "Hello World";
		myString = null;
```
[Next Lesson 2](./Lesson-2.md)
