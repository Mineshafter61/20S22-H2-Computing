# Problem Solving and Algorithm Design
===
## System Development Life Cycle (SDLC)
1. **Research:** Determine the scope of the requirements and data flows
2. **Analysis:** Think logically about how the problem can be decomposed into smaller parts.
3. **Design:** Apply abstraction (Object-Oriented Programming) to focus on important parts while hiding unnecessary details.
4. **Development/Production:** Create an algorithm to solve the problem
5. **Testing:** Test the algorithm for any errors
6. **Documentation:** what you're reading now, not covered :P
7. Implementation
8. Evaluation

## Section 1: Algorithms and Data Structures
Overview:
* Implementation of data structures
* Algorithms
* Problem decomposition and modularity
* Testing techniques (e.g. decision tables)

**Algorithm definition:** A *well-ordered* collection of *unambiguous* and *effectively computable operations* that when executed, *produces a result* and *halts in a finite amount of time*.

**Algorithms are written in _Structured English_ or _Pseudocode_, and can be represented using a _flowchart_.**

## Atomic Data Types
Pseudocode | Python | C++ | What it is
--- | --- | ---
INTEGER | int (Integer) | int, long, long long | An integer.
REAL | float | float, double | A real number. Aka number with decimal point
CHAR | str (string) | char | Any unicode character
STRING | str | string▴ | A set of characters. Not a CharArray!!!
BOOLEAN | bool | boolean | TRUE or FALSE. Nothing else.
DATE | (none) | (none) | A date.

## Identifiers
Identifiers are **names** given to **variables**. In Pseudocode, they can only contain letters (A-Z, a-z), digits (0-9) and underscores (\_). They must start with a letter and they CANNOT be a keyword (e.g. IF).
#### Pseudocode Example:
```
CTgroup ←"20S22"
```
#### Python Example:
```python
CTgroup = "20S22"
```
Note: In the exams, the convention is to use underscores to separate words.
Note2: In Python, you can use anything in Unicode as an identifier, not just letters, digits and underscores.

## Variables
A storage location for a data value with an identifier. Basically the address of the variable.
> Insight: Variables (the generic Python term, not the header here) is stored like this:
> Address, identifier, value
> e.g. 11011, foobar, 123
> The "variable" in the header refers to the address.

## Operators
Basic arithmetic operators in Pseudocode:
* + Addition
* - Subtraction
* * Multiplication
* / Division
The list of operators may differ from language to language, but the above are the basic four that 99% of languages have.

Relational operators:
Name | Pseudocode | Python/C++
--- | --- | ---
Greater than | > | >
Less than | < | <
Greater than or equal to | >= | >=
Less than or equal to | <= | <=
Equal to | = | ==
Not equal to | <> | !=

Logical operators:
* **AND**: Gives TRUE when BOTH booleans are TRUE
* **OR**: Gives TRUE when ONE boolean is TRUE
* **NOT**: Inverts boolean

## Functions
Functions are blocks of code that give a result when called, similar to f(x) in math.
**For example:**
Pseudocode:
```
GIVENAME(name: STRING) RETURNS STRING
  Concatenates "Hello " and the STRING name.
  Example: GIVENAME(Mike) returns "Hello Mike".
```
Python:
```python
def giveName(name):
  return "Hello " + name;
```

## How variables are stored
```python
a = 5
```
1. When a variable is assigned a data value, the data value is moved from the static to the register. The data value is recognised by its address (e.g. E101).
2. The value in the register is then moved to the RAM through the data bus. The location in the RAM is given by the address bus.

### Storing of variable with manipulation to data value
```python
a = a + 8
```
1. Same as step 1 above.
2. The values that will change the original value is also stored in the register. 
3. The original value is manipulated and stored to the register.
4. Same as step 2 above.
