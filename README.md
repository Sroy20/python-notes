If you are planning to give a coding interview in Python, remembering the information presented below will be beneficial.

## Mutable, Hashable, and Iterable

**Mutable/Immutable**: In Python, some objects are mutable, meaning they can be altered.  Others are immutable; they cannot be changed but rather return new objects when attempting to update. 

The following are some immutable objects: int, float, decimal, complex, bool, string, tuple, range, frozenset, bytes

The following are some mutable objects: list, dict, set, array.array, bytearray, user-defined classes (unless specifically made immutable)

The way I like to remember which types are mutable and which are not is that containers and user-defined types tend to be mutable while scalar types are almost always immutable. Then remember some notable exceptions: tuple is an immutable container, frozenset by definition is an immutable version of set. Strings are immutable. 

It is important to understand Mutability for writing efficient codes. For example, concatenating two strings or adding a new elemnent to a tuple creates a new object and hence is memory inefficient.

**Hashable**: An object is hashable if it has a hash value which never changes during its lifetime (it needs a __hash__() method), and can be compared to other objects (it needs an __eq__() or __cmp__() method). In addition, hashable objects which compare equal must have the same hash value.

Hashability makes an object usable as a dictionary key and a set member, because these data structures use the hash value internally.

All of Python’s immutable built-in objects are hashable, while no mutable containers (such as lists or dictionaries) are. Objects which are instances of user-defined classes are hashable by default; they all compare unequal, and their hash value is their id().

## Python Data Structures

### List
dw
