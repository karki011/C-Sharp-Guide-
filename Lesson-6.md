# C# Properties
---
### Properties overview
* Properties enable a class to expose a public way of getting and setting values, while hiding implementation or verification code.
* A get property accessor is used to return the property value, and a set property accessor is used to assign a new value
* Properties can be read-write (they have both a get and a set accessor).
* Property accessors often consist of single-line statements that just assign or return the result of an expression.
`    public string Name => $"{firstName} {lastName}";   `
```
using System;

class TimePeriod
{
   private double seconds;

   public double Hours
   {
       get { return seconds / 3600; }
       set {
          if (value < 0 || value > 24)
             throw new ArgumentOutOfRangeException(
                   $"{nameof(value)} must be between 0 and 24.");

          seconds = value * 3600;
       }
   }
}

class Program
{
   static void Main()
   {
       TimePeriod t = new TimePeriod();
       // The property assignment causes the 'set' accessor to be called.
       t.Hours = 24;

       // Retrieving the property causes the 'get' accessor to be called.
       Console.WriteLine($"Time in hours: {t.Hours}");
   }
}
// The example displays the following output:
//    Time in hours: 24

```
---

### Interface Properties
* Properties can be declared on an interface.
```
public interface ISampleInterface
{
    // Property declaration:
    string Name
    {
        get;
        set;
    }
}

```
* interface  can be subclass of another interface
* little more abstract than class
* is a blueprint
* merely requires **implemented** does not care how it is **implementation**.
* best practice to start by uppercase I
* benefit conform to multiple interfaces.
* cannot be private can be internal , public interface
