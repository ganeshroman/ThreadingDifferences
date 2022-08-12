

## Differences

<img src="https://dz2cdn1.dzone.com/storage/temp/13990723-java-collection-hierarchy.jpeg">




### ArrayList
ArrayList is implemented as a resizable array. as more elements are added to arraylist, its size is increased dynamically. it's elements can be accessed directly by using the get and set methods, since arraylist is essentially an array.
The default initial capacity of an arraylist is pretty small.
It is a good habit to construct the arraylist with a higher initial capacity. this can avoid the resizing cost.


## LinkedList
LinkedList is implemented as a double linked list. its performance on add and remove is better than arraylist, ***but worse on get and set methods.***


### Vector
Vector is similar with ArrayList, but it is ***synchronized***.
vector each time doubles its array size, while arraylist grow 50% of its size each time. 



### Performance of ArrayList vs. LinkedList

|   | ArrayList | LinkedList  |
|----|----------|:-----------:|
| get()  | O(1)  | O(n)   |
| add()  | O(1)   | O(1) amortized  |
|  remove() | O(n)   | O(n)   |
|   |   |   |





