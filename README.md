Aryan KC - axk220274
CS 3345.002 (Data Structures and Intro to Algorithmic Analysis)
Project 2 - Lazy Binary Search Tree - Professor Satpute

Instructions to Compile and Run:

1. Make sure the following files are in the same directory:
   - LazyBinarySearchTree.java
   - LazyBSTMain.java
   - input.txt (your input file)

2. Compile:
   javac LazyBinarySearchTree.java LazyBSTMain.java

3. Run:
   java LazyBSTMain input.txt output.txt
   if OnlineGDB - just enter input.txt output.txt in command line

Description:
- This program builds and manages a Lazy Binary Search Tree using input.
- Implemented and tested using Visual Studio Code (VSCode).
- It reads commands from input.txt and writes results to output.txt.
- Works with all commands specified in instructions, insert, delete, contains, printtree, findmin / max,
   height, and size.
- All key-based operations only accept values in the range [1, 99], 
   any key outside this range throws an IllegalArgumentException.
- Invalid lines or unrecognized commands result in: Error in line: <command>

- Edge Case Examples:
  - Insert:132      -> Error: key out of range
  - Delete:0        -> Error: key out of range
  - Insert:55 followed by Insert:55  -> Second insert returns False
  - Delete:55 then Contains:55 -> Returns False (lazy deletion)
  - FindMin after deleting all nodes -> Returns -1
  - FindMax on an empty tree -> Returns -1
  - Insert:-5       -> Throws IllegalArgumentException
  - Insert:abc      -> Causes parsing error (caught and logged)


