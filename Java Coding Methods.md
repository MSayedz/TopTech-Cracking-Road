# Java Methods:

## Methods of Collection
The Collection interface includes various methods that can be used to perform different operations on objects. These methods are available in all its subinterfaces.

      add()       inserts the specified element to the collection
      remove()    removes the specified element from the collection
      size()      returns the size of the collection
      iterator()  returns an iterator to access elements of the collection
      addAll()    adds all the elements of a specified collection to the collection
      removeAll() removes all the elements of the specified collection from the collection
      clear()     removes all the elements of the collection

## Methods of List
The List interface includes all the methods of the Collection interface. Its because Collection is a super interface of List.

Some of the commonly used methods of the Collection interface that's also available in the List interface are:

      get()       helps to randomly access elements from lists
      set()       changes elements of lists
      toArray()   converts a list into an array
      contains()  returns true if a list contains specified element
      
      + Collection Interface Methods 
      add()       adds an element to a list
      addAll()    adds all elements of one list to another
      size()      returns the length of lists
      iterator()  returns iterator object that can be used to sequentially access elements of lists
      remove()    removes an element from the list
      removeAll() removes all the elements from the list
      clear()     removes all the elements from the list (more efficient than removeAll())
      

### Methods of ArrayList Class

Besides those basic methods, here are some more ArrayList methods that are commonly used.

      sort()	Sort the arraylist elements.
      clone()	Creates a new arraylist with the same element, size, and capacity.
      isEmpty()	Checks if the arraylist is empty.
      indexOf()	Searches a specified element in an arraylist and returns the index of the element.
      contains()	Searches the arraylist for the specified element and returns a boolean result.
      ensureCapacity()	Specifies the total element the arraylist can contain.
 
   * Create an ArrayList from an Array
      
          ArrayList<String> arrayList = new ArrayList<>(Arrays.asList(array));
      
   * Create and initialize ArrayList
      
         ArrayList<String> animals = new ArrayList<>(Arrays.asList("Cat", "Cow", "Dog"));

### Methods of Vector

The Vector class also provides the resizable-array implementations of the List interface (similar to the ArrayList class). Some of the Vector methods are:

   * Add Elements to Vector

            add(element)            adds an element to vectors
            add(index, element)     adds an element to the specified position
            addAll(vector)          adds all elements of a vector to another vector
            
   * Access Vector Elements

            get(index)              returns an element specified by the index
            iterator()              returns an iterator object to sequentially access vector elements
            
   * Remove Vector Elements
   
            remove(index)           removes an element from specified position
            removeAll()             removes all the elements
            clear()                 removes all elements. It is more efficient than removeAll()
            
   * Others Vector Methods
   
            set()	                  changes an element of the vector
            size()	            returns the size of the vector
            toArray()	            converts the vector into an array
            toString()	            converts the vector into a String
            contains()	            searches the vector for specified element and returns a boolean result

### Stack Methods
Since Stack extends the Vector class, it inherits all the methods Vector. To learn about different Vector methods, visit Java Vector Class.

      push()      Method To add an element to the top of the stack
      pop()       Method To remove an element from the top of the stack
      peek()      Method to returns an object from the top of the stack without removing it
      search()    Method To search an element in the stack, It returns the position of the element from the top of the stack
      empty()     Method To check whether a stack is empty or not

 Use ArrayDeque Instead of Stack
 To implement a LIFO (Last-In-First-Out) stacks in Java, it is recommended to use a deque over the Stack class. The ArrayDeque class is likely to be faster than the Stack class.
 
 ArrayDeque provides the following methods that can be used for implementing a stack.

      push()      adds an element to the top of the stack
      peek()      returns an element from the top of the stack
      pop()       returns and removes an element from the top of the stack
      
### Methods of Queue

The Queue interface includes all the methods of the Collection interface. It is because Collection is the super interface of Queue.

Some of the commonly used methods of the Queue interface are:

      add()       Inserts the specified element into the queue. If the task is successful, add() returns true, if not it throws an exception.
      offer()     Inserts the specified element into the queue. If the task is successful, offer() returns true, if not it returns false.
      element()   Returns the head of the queue. Throws an exception if the queue is empty.
      peek()      Returns the head of the queue. Returns null if the queue is empty.
      remove()    Returns and removes the head of the queue. Throws an exception if the queue is empty.
      poll()      Returns and removes the head of the queue. Returns null if the queue is empty.
 
      
 ### Methods of Deque

Since Deque extends the Queue interface, it inherits all the methods of the Queue interface.

Besides methods available in the Queue interface, the Deque interface also includes the following methods:

      addFirst()        Adds the specified element at the beginning of the deque. Throws an exception if the deque is full.
      addLast()         Adds the specified element at the end of the deque. Throws an exception if the deque is full.
      offerFirst()      Adds the specified element at the beginning of the deque. Returns false if the deque is full.
      offerLast()       Adds the specified element at the end of the deque. Returns false if the deque is full.
      getFirst()        Returns the first element of the deque. Throws an exception if the deque is empty.
      getLast()         Returns the last element of the deque. Throws an exception if the deque is empty.
      peekFirst()       Returns the first element of the deque. Returns null if the deque is empty.
      peekLast()        Returns the last element of the deque. Returns null if the deque is empty.
      removeFirst()     Returns and removes the first element of the deque. Throws an exception if the deque is empty.
      removeLast()      Returns and removes the last element of the deque. Throws an exception if the deque is empty.
      pollFirst()       Returns and removes the first element of the deque. Returns null if the deque is empty.
      pollLast()        Returns and removes the last element of the deque. Returns null if the deque is empty.
   
   
## Coding Library

 [Main programiz.com](https://www.programiz.com/java-programming/library)  
  
 [String](https://www.programiz.com/java-programming/library/string/compareto)  
 
 [ArrayList](https://www.programiz.com/java-programming/library/arraylist/addall)    
 
 [HashMap](https://www.programiz.com/java-programming/library/hashmap/clone)      
 
 [Math](https://www.programiz.com/java-programming/library/math/abs)        
 
 [Object](https://www.programiz.com/java-programming/library/object/hashcode)

 
