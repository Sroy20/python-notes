# python-coding-interview-notes
If you are planning to give a coding interview in Python, remembering the information presented below will be beneficial.

**Mutable/Immutable**: In Python, some objects are mutable, meaning they can be altered.  Others are immutable; they cannot be changed but rather return new objects when attempting to update. 

The following are some immutable objects:

* int
* float
* decimal
* complex
* bool
* string
* tuple
* range
* frozenset
* bytes

The following are some mutable objects:

* list
* dict
* set
* bytearray
* user-defined classes (unless specifically made immutable)

The way I like to remember which types are mutable and which are not is that containers and user-defined types tend to be mutable while scalar types are almost always immutable. Then remember some notable exceptions: tuple is an immutable container, frozenset is an immutable version of set. Strings are immutable. 

It is important to understand Mutability for writing efficient codes. For example, concatenating two strings or adding a new elemnent to a tuple creates a new object and hence is memory hungry.
