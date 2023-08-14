# Software 1 - Class Exercise 5
## Goals
- Use an extension method to add functionality to a class you wouldn't normally have access to.

## Instructions
We're going to extend `List` to check for in stock items.  This is a check that we would potentially do a lot in the future of our program.  So adding a method to do this will make the code more readable and easier to maintain.
1. Create a new `static` class.  Call it `ListExtensions`.
1. In this class we're going to create a static method.  This one will be kind of complicated, so here's the method _signature_: `public static List<T> InStock<T>(this List<T> list) where T: Product`. 
1. Your mentors should have explained a little bit about _generics_.  They're not critical to understanding extension methods, but hopefully it will take some of the mystery out of how the method is working.  You'll learn much more about generics in the next course.
1. In the method body, return the "in stock" code we wrote last time.  Since this method is returning a list, remember to add the `ToList` at the end.
1. We can now use this new method in our `ProductLogic` class.  Go replace the "in stock" logic with this new method.
1. Add a new method (don't forget the interface) called `GetTotalPriceOfInventory`.  It will return a decimal.  Use your new `InStock` method, the `Select` method, and the `Sum` method to get your result.
1. Add a new UI option for the new method.
1. Now just test to make sure it works correctly.
