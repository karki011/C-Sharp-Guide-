# Generic Classes
---
## Uses case of generic classes

1. Generic Classes have types parameter.
2. Generic classes and methods combine reusability, type safety and efficiency in a way that their non-generic counterparts cannot.
3. The most frequently used with collections and the methods that operate on them.
4. Use generic types to maximize code reuse, type safety, and performance.
5. Information on the types that are used in a generic data type may be obtained at run-time by using reflection

````
class TestGenericList
{
    static void Main()
    {
        // int is the type argument
        GenericList<int> list = new GenericList<int>();

        for (int x = 0; x < 10; x++)
        {
            list.AddHead(x);
        }

        foreach (int i in list)
        {
            System.Console.Write(i + " ");
        }
        System.Console.WriteLine("\nDone");
    }
}

```
