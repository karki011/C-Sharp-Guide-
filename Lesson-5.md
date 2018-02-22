# C# Classes
---
### What is class?
* A class is like a blueprint. It defines the data and behavior of a type.
* A class is a construct that enables you to create your own custom types by grouping together variables of other types, methods and events.
* A class keyword is a _class_.
* A class defines a type of object, but it is not an object itself.
* Class is noun in your solution.


```
public class Person
{
    // Field
    public string name;

    // Constructor that takes no arguments.
    public Person()
    {
        name = "unknown";
    }

    // Constructor that takes one argument.
    public Person(string nm)
    {
        name = nm;
    }

    // Method
    public void SetName(string newName)
    {
        name = newName;
    }
}
class TestPerson
{
    static void Main()
    {
        // Call the constructor that has no parameters.
        Person person1 = new Person();
        Console.WriteLine(person1.name);

        person1.SetName("John Smith");
        Console.WriteLine(person1.name);

        // Call the constructor that has one parameter.
        Person person2 = new Person("Sarah Jones");
        Console.WriteLine(person2.name);

        // Keep the console window open in debug mode.
        Console.WriteLine("Press any key to exit.");
        Console.ReadKey();
    }
}
// Output:
// unknown
// John Smith
// Sarah Jones

```
---
### What is Object?

* An object is a concrete entity based on a class, and is sometimes referred to as an instance of a class.

---

### Inheritance
* Inheritance is a way to reuse code by existing objects. Inheritance enables new class to receive or inherit the properties and methods of existing class. Inheritance is concept child class can inherits  its functionality of parents class.
```
public class Animal
{
    public string Name { get; set; }

    public void SayName()
    {
        Console.WriteLine("My name is " + Name);
    }
}

// The Dog class is a child class of the parent Animal class
public class Dog : Animal
{

}
```
---
## Object initializer
* An object initializer is code that runs on an object after a constructor and can be used to succinctly set any number of fields on the object to specified values. The setting of these fields occurs after the constructor is called.

```
Person p = new Person { Name = "a", Age = 23 };
//this is what an object initializer essentially does:

Person tmp = new Person(); //creates temp object calling default constructor
tmp.Name = "a";
tmp.Age = 23;
p = tmp;
```
---

### Constructor
* A constructor is a defined method on a type which takes a specified number of parameters and is used to create and initialize an object.
*  Constructors enable the programmer to set default values, limit instantiation, and write code that is flexible and easy to read.

```
public class Animal
{
    public string Name { get; set; }

    // Default, standard constructor
    public Animal() : this("Fido")
    {
        // Handle some default execution
        // this("Fido") calls the constructor below
    }

    // Specific constructor, called above as well
    public Animal(string name)
    {
        Name = name;
    }
}
```

[Next Lesson 6](./Lesson-6.md)
