The book Java Generics and Collections has this information (pages: 188, 211, 222, 240).

Data Structures :
	
					Get/Contains 		Add/Remove
	
	Array 				Θ(1) 	Θ(n) 		Θ(n)
	Stack 				Θ(n)			Θ(1)
	Queue 				Θ(n) 			Θ(1)
	Singly-Linked List 		Θ(n)			Θ(1)
	Doubly-Linked List 		Θ(n)			Θ(1)

					Get/Contains/Add/Remove
	B-Tree 				Θ(log(n))
	Red-Black Tree 			Θ(log(n))
	Splay Tree 			Θ(log(n))
	AVL Tree 			Θ(log(n))

					Get/Contains/Add/Remove	
					Average				Worst
	Hash Table 			Θ(1) 				O (n)
	Skip List 			Θ(log(n))  			O (n)
	Binary Search Tree 		Θ(log(n))  			O (n)
	KD Tree 			Θ(log(n)) 			O (n)


List implementations:

	                      Get  Add  Contains next remove(0) iterator.remove
	ArrayList             O(1) O(1) O(n)     O(1) O(n)      O(n)
	LinkedList            O(n) O(1) O(n)     O(1) O(1)      O(1)
	CopyOnWrite-ArrayList O(1) O(n) O(n)     O(1) O(n)      O(n)
	
List: A list is an ordered collection of elements.
						
				Add/Remove 	Get/Contains 	Data Structure
	LinkedList 		O (1) 		O (n) 	 		Linked List
	ArrayList 		O (1) O (n) 	O (1) 	O (n) 		Array

					

Set implementations:

	                      add      contains next     notes
	HashSet               O(1)     O(1)     O(h/n)   h is the table capacity
	LinkedHashSet         O(1)     O(1)     O(1) 
	CopyOnWriteArraySet   O(n)     O(n)     O(1) 
	EnumSet               O(1)     O(1)     O(1) 
	TreeSet               O(log n) O(log n) O(log n)
	ConcurrentSkipListSet O(log n) O(log n) O(1)
	
Set: A collection that contains no duplicate elements. O(1)
						
				Add/Contains/Next 		Data Structure
	LinkedHashSet 		O(1)				Hash Table + Linked List
	EnumSet	 		O(1)				Bit Vector
	TreeSet 		O(log n) 			Red-black tree

				Add/Contains 	Next 
	HashSet 		O(1) 	 	O(h/n) 		Hash Table
	CopyonWriteArraySet 	O(n) 		O(1) 		Array
	ConcurrentSkipList 	O(log n)	O(1) 		Skip List


Map implementations:

	                    	Get      containsKey   next     Notes
	HashMap               	O(1)     O(1)        O(h/n)   h is the table capacity
	LinkedHashMap        	O(1)     O(1)        O(1) 
	IdentityHashMap       	O(1)     O(1)        O(h/n)   h is the table 
	EnumMap               	O(1)     O(1)        O(1) 
	TreeMap               	O(log n) O(log n)    O(log n) 
	ConcurrentHashMap     	O(1)     O(1)        O(h/n)   h is the table 
	ConcurrentSkipListMap 	O(log n) O(log n)    O(1)
	
Map: An object that maps keys to values.
A map cannot duplicate keys; each key can map to at most one value.
				
				Get/ContainsKey/Next 			Data Structure
	EnumMap 		O(1) 					Array
	LinkedHashMap 		O(1) 					Hash Table + Linked List
	TreeMap 		O(log n) 				Red-black tree

				Get/ContainsKey		Next 
	IdentityHashMap 	O(1) 			O(h / n) 	Array
	HashMap 		O(1) 			O(h / n) 	Hash Table
	WeakHashMap 		O(1) 			O(h / n) 	Hash Table
	ConcurrentHashMap 	O(1) 			O(h / n) 	Hash Table
	ConcurrentSkipListMap 	O(log n) 		O(1) 		Skip List

Queue implementations:

	                    	offer    peek 	poll	 size
	LinkedList            	O(1)     O(1) 	O(1)     O(1)
	ArrayDeque            	O(1)     O(1) 	O(1)     O(1)
	PriorityQueue         	O(log n) O(1) 	O(log n) O(1)
	DelayQueue            	O(log n) O(1) 	O(log n) O(1)
	
	LinkedBlockingDeque   	O(1)     O(1) 	O(1)     O(1)
	LinkedBlockingQueue   	O(1)     O(1) 	O(1)     O(1)
	ArrayBlockingQueue    	O(1)     O(1) 	O(1)     O(1)
	ConcurrentLinkedQueue 	O(1)     O(1) 	O(1)     O(n)
	PriorityBlockingQueue 	O(log n) O(1) 	O(log n) O(1)

##############################################################

Sort :
				
				Best/Average/Worst					Space Complexity

	Merge Sort 		O ( n log(n) )						O(n)
	Heap Sort 		O ( n log(n) )						O(1)
	Selection Sort 		O ( n2 )						O(1)
	Counting Sort 		O ( n+k )						O(k)	
			
				Best/Average   		Worst
	Quick Sort 		Θ ( n log(n) ) 		O ( n2 ) 			O(log(n))
	Tree Sort 		Θ ( n log(n) ) 		O ( n2 )			O(n)

				Best			Average/Worst
	Bubble Sort 		Ω ( n ) 		O ( n2 )			O(1)
	Insertion Sort 		Ω ( n ) 		O ( n2 )			O(1)
	Timsort 		Ω ( n ) 		O ( n log(n) )			O(n)
	Cubesort 		Ω ( n ) 		O ( n log(n) )			O(n)
	Smooth Sort 		Ω ( n ) 		O ( n log(n) )
	Odd – Even sort 	Ω ( n ) 		O ( n2 )


##############################################################

Searching Algorithms:		

					Time Complexity


	Binary Search 			O ( log (n) )
	Exponential Search 		O ( log (n) )
	
	Linear Search 			O (n)
	Sequential search 		O (n)
	Interpolation Search 		O (n)
	Jump Search 			O (√ n)

	Depth-first   search (DFS) 	O ( |V| + |E| )
	Breadth-first search (BFS) 	O ( |V| + |E| )


##############################################################

