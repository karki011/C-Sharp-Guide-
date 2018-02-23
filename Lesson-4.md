# C# Statements
---
### Scope:
#### Also called block, s defined with curly braces.
---

## Selection == all about choosing what to execute.
---
### **if**
##### evaluates a condition which either resolve **true** or **false**.

### **else**
#####  used in tandem with an if statement, providing scope for an if statement that resolves to false:

```
if (4 == 5) // your conditional is "if 4 equals 5", which is false
{
    // so your if scope is skipped over
}
else
{
    // your else scope will be executed
}

```

### if-else

```
var a = 4;
var b = 5;

if (a == b) // checked first
{
    // executes if a equals b
}
else if (a > b) // checked if the first conditional isn't true
{
    // executes if the a > b
}
else
{
    // executes if all if conditionals above are false
}
```
---
## Iteration  --- statements are all about executing something multiple times

---
### while
##### Use a while loop if you need to execute some code until something happens:

```
int counter = 0;
while (counter < 10)
{
  Console.WriteLine($"Hello World! The counter is {counter}");
  counter++;
}

```
---
### do - while
##### execute the scope of the loop at lease once and keeps executing until something happens.

```
int counter = 0;
do
{
  Console.WriteLine($"Hello World! The counter is {counter}");
  counter++;
} while (counter < 10);

```
---
### for
#### if you need to execute some block of code a specific number of times:
#### There are 3 parts to a for loop
* Initializer: var i = 0
* Conditional: i < 10
* Increment: i++
```
for (var i = 0; i < 10; i++)
{
    // Execute some code
}

```
---

### foreach
#### if you need to execute some code on each element in a collection of elements.
```
var emails = new [] { "a@me.com", "b@me.com" };

foreach (var email in emails)
{
    //do something with the `email`, like send a marketing message
}

```
---

[Next Lesson 5: Classes](./Lesson-5.md)
