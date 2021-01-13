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
   

### Methods of ArrayDeque
The ArrayDeque class provides implementations for all the methods present in Queue and Deque interface.

Insert Elements to Deque
   1. Add elements using add(), addFirst() and addLast()

            add() - inserts the specified element at the end of the array deque
            addFirst() - inserts the specified element at the beginning of the array deque
            addLast() - inserts the specified at the end of the array deque (equivalent to add())
Note: If the array deque is full, all these methods add(), addFirst() and addLast() throws IllegalStateException.

   2. Insert elements using offer(), offerFirst() and offerLast()

            offer() - inserts the specified element at the end of the array deque
            offerFirst() - inserts the specified element at the beginning of the array deque
            offerLast() - inserts the specified element at the end of the array deque

Note: offer(), offerFirst() and offerLast() returns true if the element is successfully inserted; if the array deque is full, these methods return false.
Note: If the array deque is full

* the add() method will throw an exception
* the offer() method returns false

Access ArrayDeque Elements
   1. Access elements using getFirst() and getLast()

            getFirst() - returns the first element of the array deque
            getLast() - returns the last element of the array deque
Note: If the array deque is empty, getFirst() and getLast() throws NoSuchElementException.

   2. Access elements using peek(), peekFirst() and peekLast() method

            peek() - returns the first element of the array deque
            peekFirst() - returns the first element of the array deque (equivalent to peek())
            peekLast() - returns the last element of the array deque

Note: If the array deque is empty, peek(), peekFirst() and getLast() throws NoSuchElementException.

* Remove ArrayDeque Elements
   1. Remove elements using the remove(), removeFirst(), removeLast() method

            remove() - returns and removes an element from the first element of the array deque
            remove(element) - returns and removes the specified element from the head of the array deque
            removeFirst() - returns and removes the first element from the array deque (equivalent to remove())
            removeLast() - returns and removes the last element from the array deque

Note: If the array deque is empty, remove(), removeFirst() and removeLast() method throws an exception. Also, remove(element) throws an exception if the element is not found.

2. Remove elements using the poll(), pollFirst() and pollLast() method

            poll() - returns and removes the first element of the array deque
            pollFirst() - returns and removes the first element of the array deque (equivalent to poll())
            pollLast() - returns and removes the last element of the array deque
Note: If the array deque is empty, poll(), pollFirst() and pollLast() returns null if the element is not found.

3. Remove Element: using the clear() method

            clear() method To remove all the elements from the array deque

Iterating the ArrayDeque

            iterator() - returns an iterator that can be used to iterate over the array deque
            descendingIterator() - returns an iterator that can be used to iterate over the array deque in reverse order

Other Methods

      element()	Returns an element from the head of the array deque.
      contains(element)	Searches the array deque for the specified element.
      If the element is found, it returns true, if not it returns false.
      size()	Returns the length of the array deque.
      toArray()	Converts array deque to array and returns it.
      clone() 	Creates a copy of the array deque and returns it.

ArrayDeque as a Stack
To implement a LIFO (Last-In-First-Out) stacks in Java, it is recommended to use a deque over the Stack class. The ArrayDeque class is likely to be faster than the Stack class.

ArrayDeque provides the following methods that can be used for implementing a stack.

      push() - adds an element to the top of the stack
      peek() - returns an element from the top of the stack
      pop() - returns and removes an element from the top of the stack

### Methods of PriorityQueue

* Insert Elements to PriorityQueue

      add() - Inserts the specified element to the queue. If the queue is full, it throws an exception.
      offer() - Inserts the specified element to the queue. If the queue is full, it returns false.

The queue is rearranged to store the smallest element to the head of the queue.

* Access PriorityQueue Elements
      
      peek() method return the head element without removing it

* Remove PriorityQueue Elements

      remove() - removes the specified element from the queue
      poll() - returns and removes the head of the queue

* Iterating Over a PriorityQueue

      iterator() method to iterate over the elements of a priority queue

* Other PriorityQueue Methods

      contains(e)	Searches the queue for the specified element. If the element is found, it returns true, if not returns false.
      size()	Returns the length of the priority queue.
      toArray()	Converts a priority queue to an array and returns it.      
      isEmpty()

PriorityQueue == MinHeap 

      PriorityQueue<Integer> minHeap = new PriorityQueue<>();
      PriorityQueue<Integer> maxHeap = new PriorityQueue<>(Collections.reverseOrder());

Simple Comparator

      PriorityQueue<int[]> minHeap = new PriorityQueue<>((a, b)-> a[0] - b[0]);
      PriorityQueue<int[]> maxHeap = new PriorityQueue<>((a, b)-> b[0] - a[0]);

Heaps With inline Comparator

      PriorityQueue<Integer> minHeap= new PriorityQueue<Integer>(new Comparator<Integer>(){
         public int compare(Integer a, Integer b){
             if(a>b)
                return 1;
              else if(a<b)
                return -1;
              else
                return 0;
       }}); 
                         
      PriorityQueue<Integer> maxHeap= new PriorityQueue<Integer>(new Comparator<Integer>(){
         public int compare(Integer a, Integer b){
            if(b>a) 
               return 1;
            else if(b<a) 
               return -1;
            else 
               return 0;
       }}); 

Array Comparator

      PriorityQueue<int[]> maxHeap = new PriorityQueue<> (new Comparator<int[]>(){
        Public int compare(int[] a , int[] b){
            If(b[1] > a[1])
               return -1;
            else if(b[1] == a[1]) 
               return 0;
            else	
               return 1;
         }});
            
      PriorityQueue<Row> minHeap = new PriorityQueue<>(new Comparator<Row>() {
         @Override
         public int compare(Row r1, Row r2) {
            return count(r1.row)-count(r2.row);
      }});

PriorityQeuue with Map Example

      Queue<Map.Entry<String, Integer>> maxHeap = new PriorityQueue<>((a, b)->a.getValue() == b.getValue() 
                                          ? a.getKey().compareTo(b.getKey()) : b.getValue() - a.getValue());
      maxHeap.addAll(map.entrySet());

      while(!maxHeap.isEmpty() && k-- > 0) 
         resultList.add(maxHeap.poll().getKey());


Why Offer Not Add !
 
                 | Throws exception | Returns special value
      -------------------------------------------------------
      Insert     | add(e)           | offer(e)
      Remove     | remove()         | poll()
      Examine    | element()        | peek()


## Map

Map.Entry.comparingByValue()
      
      
      public class MapSortingExamples {
 
          public static void main(String[] args) {
            System.out.println("\nSorting using Java8 streams\n");

              sortByValueJava8Stream();
          }
 
          private static void sortByValueJava8Stream() 
          {
              Map<String, Integer> unSortedMap = getUnSortedMap();

              System.out.println("Unsorted Map : " + unSortedMap);

              LinkedHashMap<String, Integer> sortedMap = new LinkedHashMap<>();
              unSortedMap.entrySet().stream().sorted(Map.Entry.comparingByValue())
                      .forEachOrdered(x -> sortedMap.put(x.getKey(), x.getValue()));

              System.out.println("Sorted Map   : " + sortedMap);

              LinkedHashMap<String, Integer> reverseSortedMap = new LinkedHashMap<>();
              unSortedMap.entrySet().stream().sorted(Map.Entry.comparingByValue(Comparator.reverseOrder()))
                      .forEachOrdered(x -> reverseSortedMap.put(x.getKey(), x.getValue()));

              System.out.println("Reverse Sorted Map   : " + reverseSortedMap);
          }
 
          private static Map<String, Integer> getUnSortedMap() 
          {
              Map<String, Integer> unsortMap = new HashMap<>();
              unsortMap.put("alex", 1);
              unsortMap.put("david", 2);
              unsortMap.put("elle", 3);
              unsortMap.put("charles", 4);
              unsortMap.put("brian", 5);
              return unsortMap;
          }
      }


      Output:

      Sorting using Java8 streams

      Unsorted Map        : {alex=1, charles=4, david=2, brian=5, elle=3}
      Sorted Map          : {alex=1, david=2, elle=3, charles=4, brian=5}
      Reverse Sorted Map  : {brian=5, charles=4, elle=3, david=2, alex=1}


## Coding Library

 [Main programiz.com](https://www.programiz.com/java-programming/library)  
  
 [String](https://www.programiz.com/java-programming/library/string/compareto)  
 
 [ArrayList](https://www.programiz.com/java-programming/library/arraylist/addall)    
 
 [HashMap](https://www.programiz.com/java-programming/library/hashmap/clone)      
 
 [Math](https://www.programiz.com/java-programming/library/math/abs)        
 
 [Object](https://www.programiz.com/java-programming/library/object/hashcode)

 
