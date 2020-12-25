The Collection interface is the root interface of the Java collections framework.

There is no direct implementation of this interface. However, it is implemented through its subinterfaces like List, Set, and Queue.

For example, the ArrayList class implements the List interface which is a subinterface of the Collection Interface.

### Subinterfaces of Collection
As mentioned above, the Collection interface includes subinterfaces that are implemented by various classes in Java.

1. List Interface

The List interface is an ordered collection that allows us to add and remove elements like an array.

2. Set Interface

The Set interface allows us to store elements in different sets similar to the set in mathematics. It cannot have duplicate elements.

3. Queue Interface

The Queue interface is used when we want to store and access elements in First In, First Out(FIFO) manner. 

### Classes that Implement List
Since List is an interface, we cannot create objects from it.

In order to use functionalities of the List interface, we can use these classes:

  * ArrayList
  * LinkedList
  * Vector
  * Stack

### Java List vs. Set
Both the List interface and the Set interface inherits the Collection interface. However, there exists some difference between them.

Lists can include duplicate elements. However, sets cannot have duplicate elements.
Elements in lists are stored in some order. However, elements in sets are stored in groups like sets in mathematics.
