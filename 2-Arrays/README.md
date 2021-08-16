# Table of contents

1. [Definition of an Array and its main features](#)
2. [Mechanics of arrays](#)

**Interesting questions**

1. [What happens when element is inserted into the middle of an array?](#)
2. [What happens when the array exceeds its capacity and gets too big?](#)

**Definition of an Array and its main features**
Array is a collection of elements, all of the same type, that can be set and retrieved via a continous series of integers (indexes).

Example methods on Array:

```swift
let data = [Int]()
get(i)
set(i, value)
insert(i, value)
delete(i)
```

Arrays can hold any type of data

```swift
let ints = [Int]()
let strings = [String]()
let people = [Person]()
```

Arrays are of fixed size (we don't see this in Swift).

Arrays posses Random Access ability
We can get or set (set(5, "b") or get(4)) data to any index. This is big. Because data structures like: Linked Lists, Stacks and Queues and Binary Search Trees cannot do that.

get(4) or set(5, "b") has O(1) (Constant time)

**Mechanics of arrays**

- Insesrt O(n)
  When inserting an element into an array we do three things:

1. **Copying** => Copy all elements starting from inserted index and above, move them one index above and then insert the value in the index
2. Inserting
3. Incrementing

- Delete
- Resize (how arrays grow when they get big)
