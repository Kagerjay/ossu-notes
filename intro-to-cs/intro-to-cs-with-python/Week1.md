## Week 1 - First Half Notes

We can represent knowledge with data structure. These data structures eventualy make up a computer. All computers can do the following

1. **Store**
2. **Perform Calculations**

Calculations can be extremely large. World wide has 45B pages, searching it brute force is inefficient. Playing chess has many look aheads for potential moves.

Storing and indexing is not a pure solution. Some problems are still too complex to solve in real time.

To solve this, we start at beginning by defining "knowledge".

1. **Declarative knowledge** - these are statements of facts
2. **Imperative knowledge** - These are recipes from a cookbook or "how to"

A recipe is defined in a 3 step process. All 3 combined are considered an algorithm

1. Sequence of simple steps
2. Flow of control - Specifying when each step is executed
3. When to stop

Recipes are stored in machines. Machines, can be one of two seperate things

1. **Fixed program** - like a calculator (HIGH LEVEL)
2. **Stored program** - machine stores and executes instructions (LOW LEVEL)

The architecture of a machine is as follows:

![clipboard.png](https://i.imgur.com/GMoVqsq.png)
- The ALU takes information from memory
- The control unit keeps track of what ALU is doing
- Program counter points to memory

### Language

Machines program have 6 different data primitive types. At the lowest level. Modern languages have more.

These languages provide a set of **operations and expressions**. They act like components in a recipe.

An analogy to a computer recipe is like the English language. Let's look at it. English has **primitive constructs** , the most basic building block unit. For programming language, these are data types

- English: words
- Programming language: numbers, strings, simple operators

Comparing English analogy further, we define several things

- **Syntax**
  - Base rules
    - English - Nouns, verbs, etc have set of rules. "Cat dog boy" is not a valid statement
    - Programming Language - Each language is different `no spaced python, () brackets` etc. For instance, "hi"5 is not valid, but 3.2*5 is
- **Static Semantics**
  - This is where you define something with the correct intent, but did not follow the semantic rules
    - English - "I are hungry" is not ok
    - Programming - 3+"hi" is not ok, but 3.2*5 is
- **Semantics**
  - This is when you define something with many implicit meanings
    - English - e.g. I lied on the ground
    - Programming - unintentionally meaning. E.g. javascripts `this` object

### Python Programs

We move onto pytthon basics. Python works in shell or as a file. Python is two things.

- **Program** - sequence of definitions and commands. Definitions are evaluated, and commands executed by python IDLE
- **Commands** - instruct interpreter to make sense of .py file like `make`

Programs manipulate **data objects**. Objects have some specific rules, namely

- **Scalar** (cannot be subdivided). These are
  - int, float, bool, nonetype
- **nonscalar** (can be accessed externally)

Python as a language can do the following
- Convert one data type to another
- print to console
- combine expressions object and operators
- Do basic math operations
- Assign variables in memory locations

Programs follow a sequence of steps. You can have conditional statements, e.g. forks in potential operations. These are expressed as `if else if` type statements.
They run in constant time normally, since the same number of steps is taken for each pathway
