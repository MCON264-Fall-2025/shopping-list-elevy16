# Shopping List App

This project is a small console-based list application built for Data Structures course (MCON 264)
It demonstrates how to use the ***List ADT*** and how to program against an interface.

The app manages grocery items, keeps them sorted, and lets the user shop items one at a time.

---

## Features

### Add items in sorted order
Items are automatically inserted into the correct position based on aisle and item name. Sorting uses the `compareTo` method in the `ShoppingItem` class.

### View current shopping list
Items are displayed in sorted order using the `iterator()` provided by `ListInterface`.

### Shop the next item
The next item is the one at index 0, which is removed and returned.

### Switchable implementations
The app stores items using `ListInterface<ShoppingItem> shoppingList = new ArrayBasedList<>();`

---

## Programming to an Interface
This assignment shows that when your code uses the ListInterface instead of a specific class, your whole app works the same with either ArrayBasedList or LinkedBasedList.
This brings the value of flexibility and no dependency on the internal implementation.

## Using the List ADT as an Abstraction
Using an ADT hides how a data structure works internally and only exposes the operations you need.
You can just call `add`, `get`, `remove`, and `iterator()`, and the ADT handles the details.
This brings the value of simpler and cleaner code that does not have to deal with low level data structure mechanics.