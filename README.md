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
- 