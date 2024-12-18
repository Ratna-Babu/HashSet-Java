# HashSet in Java

This is a simple demonstration of using the `HashSet` class in Java to perform set operations like adding elements and finding the union of two sets.

## What is a HashSet?

A `HashSet` is a collection class in Java that implements the `Set` interface. It stores unique elements and does not allow duplicates. Internally, it uses a hash table to store the elements, which provides efficient performance for basic operations such as adding, removing, and checking the presence of elements.

### Key Features of HashSet:
- **Uniqueness**: A `HashSet` only stores unique elements (no duplicates).
- **No specific order**: The elements in a `HashSet` are unordered, meaning the order in which elements are added is not maintained.
- **Efficient operations**: It offers constant-time performance (O(1)) for basic operations like `add`, `remove`, and `contains`, assuming the hash function disperses elements properly.

## Code Explanation

In the provided Java code, we create two `HashSet` objects, `set1` and `set2`, and perform the following operations:

1. **Creating the sets**:
   - `set1` is initialized with elements `2` and `3`.
   - `set2` is initialized with elements `1` and `2`.

2. **Printing the sets**:
   - We print the contents of `set1` and `set2` to the console.

3. **Union of sets**:
   - The `addAll()` method is used to add all elements from `set1` into `set2`. This performs a union operation, ensuring that no duplicate elements are added to `set2`.

4. **Displaying the union**:
   - Finally, the union of the two sets is printed to the console.

## Key Methods in HashSet:

- **add(E e)**: Adds the specified element to the set if it is not already present.
- **addAll(Collection<? extends E> c)**: Adds all elements from the specified collection to the set, ensuring no duplicates.
- **contains(Object o)**: Checks if the set contains the specified element.
- **remove(Object o)**: Removes the specified element from the set.
- **size()**: Returns the number of elements in the set.
- **clear()**: Removes all elements from the set.
- **isEmpty()**: Checks if the set is empty.

```Code
import java.util.Set;
import java.util.HashSet;

public class HashSetDemo {
    public static void main(String[] args) {
        Set<Integer> set1 = new HashSet<>();
        set1.add(2);
        set1.add(3);
        System.out.println("Set 1:" + set1);
        Set<Integer> set2 = new HashSet<>();
        set2.add(1);
        set2.add(2);
        System.out.println("Set 2: " + set2);
        set2.addAll(set1);
        System.out.println("Union is: " + set2);
    }
}
```
## Output
```
Set 1:[2, 3]
Set 2: [1, 2]
Union is: [1, 2, 3]
```

## Conclusion

`HashSet` is a powerful and efficient data structure for working with unique elements in Java. It's particularly useful when you need to perform set operations like union, intersection, and difference. The demonstration in this code shows how to use basic `HashSet` operations in Java.

Feel free to experiment with different set operations and explore how the `HashSet` class works in Java!
