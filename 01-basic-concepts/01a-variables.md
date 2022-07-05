# Variables 

[toc]

## Concepts

### Mathematical

**Variables**

>  The concept of variables predates coding through mathematics.

- **Definition**: A placeholder symbol (alias) for a changeable value (of any kind)

Take for example the quadratic function `ax^2 + bx + c` - this contains 4 different variables used in a calculation - including one used twice. These values are not known until given, so they are treated as placeholders, which helps mathematicians map trends, graphs, and solve for values where they are not given.



**Constants**

There also exists a special type of placeholder for variables that do not change, such as PI (3.14). These are called constants - their value cannot change and if it does, the equation does not work.

​	



---

### Programmatic

Variables in code are similar to mathematical variables - they are named placeholders for values. However, the value has to be stored in the computer memory, instead of on paper, so that the computer can re-read when the variable is stated again in the code.



**Variables & Constants**

- **Variables**: Mutable (changeable) placeholder values stored in memory
- **Constants**: Immutable (unchangeable) placeholder values stored in memory



**Common Operations**

- **Declaration**: Most languages contain a keyword (or syntax) to create the variable (such as `let`, `var` etc.) which will assign the variable a place in memory.
- **Assignment**: Most
- **Initialisation**
- **State**:



**Size & Storage**

Each variable will have a certain size based on the type of data it is assigned (or initialised as, depending on the language). Once the program knows how big the variable is supposed to be, it can assign a specific amount of memory to store that variable. The variable then becomes associated with a memory address on initialisation.









## Data Types

### Basics

Programming languages define a (similar set of) data types that a variable can be. They range from primary data types (such as numbers and characters - single items) that can be referenced at a single memory address, to complex types that span many, often non-linear memory-addresses.



Under the hood of the program, all these values still translate to binary, but can be interpreted to human-readable values also by the computer.



**Primary / Scalar Types**

You will alse hear these referred to as value types, as most languages will

| Data Type          | Purpose / Explanation                                        |
| ------------------ | ------------------------------------------------------------ |
| Number(s)          | Single values that have value limits which can be stored at a single memory address. many languages split the number types into integers (whole numbers), floating points (decimals) and many more! |
| Characters (chars) | These are single characters (i.e. '`a`') that represent language. While |
| Booleans           | Booleans are a type of true/false binary value (1 or 0) whereby the value is true if 1, or false if 0. |
| byte               | Actual binary - a sequence of normally 8 1's and 0's         |



**Linear Memory Types**



| Data Type | Purpose / Explanation |
| --------- | --------------------- |
| Arrays    |                       |
| Structs   |                       |





**Reference Types**

For variables that are large collections, i.e. containing lots of inner variables, that are not continuous in memory (i.e. objects), they are assigned memory in a way that is optimal for the program. They are referred to as reference types as most of the time when you create a variable, the value stored is a reference to the memory address of the object, not the object itself. (This will become clearer studying data structures).

So when you state the variable, the reference type can be de-referenced to retrieve the object and load it into memory.

> The variable of a reference type is the memory address that "grants access" to the data collection in memory. Most languages to automatic handling of reference types, but some require manual referencing and dereferencing.

---

### (Strongly) Typed & Dynamic Lanuages





























