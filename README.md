# CollectionsFramework

##### Overview :
- Arrays : 
    * The biggest advantage of arrays is, we can represent huge data set using one variable.
    * Readability of code increase, as we don't have to individually represent the data.
    * Arrays are fixed in size, once created, there is no chance of increasing/decreasing its size.
    * Arrays can hold only homogeneous data elements.
    * Arrays concept is not implemented based on some standard data structure.
    * Readymade method support for arrays we can't expect.

```
Student[] students = new Student[10];
students[0] = new Student();
// incompatible type found, homogeneous data element is required.
students[1] = new Customer();

// valid data elements
Object[] objects = new Object[10];
objects[0] = new Student();
objects[1] = new Customer();
```

##### Collections :
- Collections are growable in nature. (We can overcome the problem of increasing/decreasing the capacity of array).
- Collections can hold both homogeneous & heterogeneous objects.
- Every collection class is based on some standard data structure.
- Readymade method support is available, hence we don't have to explicitly write implementations.


##### Difference between Arrays & Collections :
- Arrays are fixed in size.
- Collections are growable in nature.

- Arrays are not great w.r.t to memory, allocating more memory locations is not possible.
- Collections have that support of increasing memory support for additional data elements.

- w.r.t performance, arrays are recommended.
- w.r.t performance, collections are not recommended.

- Arrays can hold only homogeneous elements.
- Collections can hold both.

- Since Arrays concept is not based on some standard D.S, underlying D.S support is not available, readymade method support is also not available.
- For every collection, readymade method support is available.

- By using arrays, we can use primitives & non-primitives array types.
- By using collections, we can hold only objects but not primitives.

```
int[] array = new int[100];
Integer[] array = new Integer[100];

List<Integer> bag = new ArrayList();
List<int> bag = new ArrayList(); // not allowed
```

- Note : the above explaination is valid for :
    * Arrays vs ArrayList
    * Arrays vs Vector  
    * Arrays vs TreeSet and so on...

##### Collection & Collections Framework :
- Collection is a group of individual objects as single entity.
- Collections Framework defines several classes & interfaces which can be used to represent collection.
- Collection interface defines the most common methods which are applicable for any Collection object.
- In general, collection interface is considered as root interface of Collection Framework.
- Note : There is no concrete class which implements Collection Interface directly.

##### Difference between Collection & Collections :
- Collection is an interface, Collections is a bunch of classes.
- When we want to represent individual objects as single entity, we use Collection. Whereas Collections is a utility class, which defines bunch of methods to interact with Collection and defines utility methods for Searching, Sorting etc.

##### Interfaces & Heirarchy :
- Collection, List, ArrayList, LinkedList came in Java V1.2.
- Vector, Stack came in Java V1.0, and so they are legacy classes.

![github-small](images/one.png)

- Set, HashSet, LinkedHashSet.

![github-small](images/two.png)

##### Differences between List & Set :
- List : Duplicates are allowed.
- Set : Duplicates are not allowed.

- List : Insertion order is preserved.
- Set : Insertion order is not preserved.

##### SortedSet, NavigableSet : 
- SortedSet : It we want to treat individual objects as single entity where duplicates are not allowed but all objects should be inserted according to some sorting order then we should go for SortedSet.
- NavigableSet (Child interface of SortedSet) :
    * It defines certain methods for navigation purpose.
    * For example : nextElement, previousElement.
    * TreeSet is the implementation class of NavigableSet.

![github-small](images/three.png)

##### Queue :
- Queue comes from Collection interface.
- Its child interfaces are :
    * PriorityQueue
    * BlockingQueue (interface) :
        * LinkedBlockingQueue
        * PriorityBlockingQueue

![github-small](images/four.png)

- Note : All the above interfaces are meant for representing a group of individual objects. If we want to represent a group of objects as key-value pairs, then we should go for Map Interface.

##### Map :

![github-small](images/five.png)

![github-small](images/six.png)

![github-small](images/seven.png)

##### Overview of Collections Framework (Entirely):
