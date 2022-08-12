

## Differences

<img src="https://dz2cdn1.dzone.com/storage/temp/13990723-java-collection-hierarchy.jpeg">




### ArrayList
ArrayList is implemented as a resizable array. as more elements are added to arraylist, its size is increased dynamically. it's elements can be accessed directly by using the get and set methods, since arraylist is essentially an array.
- The default initial capacity of an arraylist is pretty small.
- It is a good habit to construct the arraylist with a higher initial capacity. this can avoid the resizing cost.


## LinkedList
LinkedList is implemented as a double linked list. its performance on add and remove is better than arraylist, ***but worse on get and set methods.***


### Vector
Vector is similar with ArrayList, but it is ***synchronized***.
- vector each time doubles its array size, while arraylist grow 50% of its size each time. 



### Performance of ArrayList vs. LinkedList

|   | ArrayList | LinkedList  |
|----|----------|:-----------:|
| get()  | O(1)  | O(n)   |
| add()  | O(1)   | O(1) amortized  |
|  remove() | O(n)   | O(n)   |




### HashSet, LinkedHashSet & TreeSet Difference

| Features | HashSet | LinkedHashSet | TreeSet |
|----------|:-------:|---------------|---------|
| Internal Working | HashSet internally uses HashMap for storing objects | LinkedHashSet uses LinkedHashMap internally to store objects | TreeSet uses TreeMap internally to store objects |
| When To Use | If you don’t want to maintain insertion order but want to store unique objects | If you want to maintain the insertion order of elements then you can use LinkedHashSet | If you want to sort the elements according to some Comparator then use TreeSet | 
| Order | HashSet does not maintain insertion order | LinkedHashSet maintains the insertion order of objects | While TreeSet orders the elements according to supplied Comparator. By default, objects will be placed according to their natural ascending order. |
|Complexity of Operations |HashSet gives O(1) complexity for insertion, removing, and retrieving objects |LinkedHashSet gives insertion, removing, and retrieving operations performance in order O(1).|While TreeSet gives the performance of order O(log(n)) for insertion, removing, and retrieving operations. |
| Performance | The performance of HashSet is better when compared to LinkedHashSet and TreeSet. | The performance of LinkedHashSet is slower than TreeSet. It is almost similar to HashSet but slower because LinkedHashSet internally maintains LinkedList to maintain the insertion order of elements| TreeSet performance is better than LinkedHashSet except for insertion and removal operations because it has to sort the elements after each insertion and removal operation.|
| Compare | HashSet uses equals() and hashCode() methods to compare the objects | LinkedHashSet uses equals() and hashCode() methods to compare it’s objects |TreeSet uses compare() and compareTo() methods to compare the objects |
| Null Elements | HashSet allows only one null value. | LinkedHashSet allows only one null value. | TreeSet does not permit null value. If you insert null value into TreeSet, it will throw NullPointerException. |
|Syntax | HashSet obj = new HashSet(); | LinkedHashSet obj = new LinkedHashSet(); | TreeSet obj = new TreeSet();|






