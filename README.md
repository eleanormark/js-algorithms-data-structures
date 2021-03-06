js-algorithms-data-structures
=============================

Using javascript to implement data structures, algorithms, and common interview
problems. This is for those who are front-end engineers who don't have comp sci
degrees, but may be applying for a front-end position where the interviewer
expects this knowledge.

I've been following Cracking the Coding Interview and Data Structures and
Algorithms in Javascript for this preparation. CCI solutions are implemented
in Java, so I have tackled them in javascript and then made revisions of the
solution in javascript. DSAJ data structures and tests are taken from the book
but I have commented (and corrected mistakes!) on the code to ensure I am
understanding each line thoroughly.

Usage:
======

Most of the scripts with the exception of the scripts in the `inbrowser` folder
are meant to be run using the included js executable. They are all in the `scripts`
folder. Right now they're just loosely organized. "ADT" means abstract data type
and that file is likely loaded by another script that is running an alg or test.

Just run:

`./js scripts/PATH_OR_FILENAME_OF_JS_FILE`

The `inbrowser` files are meant to be opened in a browser.

Also added some other miscellaneous notes to help me in an interview.

Notes:
======

Some other problems to try:

- Write a function that takes two sorted lists of numbers and merges them into a single sorted list.
- Given an input array and another array that describes a new index for each element, mutate the input array so that each element ends up in their new index. Discuss the runtime of the algorithm and how you can be sure there won't be any infinite loops
- In JavaScript, write a function that takes an array as input that can contain both ints and more arrays (which can also contain an array or int) and return the flattened array.

ex. [1, [2, [ [3, 4], 5], 6]] => [1, 2, 3, 4, 5, 6]
- Determine if a given string is an anagram of another.
O Implement a function that finds the square root in javascript.
- Given an array of integers (positive or negative) find the sub-array with the largest sum.
- Determine if a given string is a palindrome.
- Given a large hash table whose keys are movie names and whose values are a list of actors in those movies, write a function to determine the Bacon number of a particular actor.
- Given two nodes in a binary search tree, find the lowest common ancestor of the two nodes.
X Design the data structures and algorithms to detect typos in a document and then provide suggestions to the user.
- Write a function to reverse a string.
- Write function to compute Nth fibonacci number.
- Print out the grade-school multiplication table up to 12x12.
- Write a function that sums up integers from a text file, one int per line.
- Write function to print the odd numbers from 1 to 99.
- Find the largest int value in an int array. 
- Format an RGB value (three 1-byte numbers) as a 6-digit hexadecimal string.
- Design a deck of cards that can be used for different card game applications. 
- Model the Animal kingdom as a class system, for use in a Virtual Zoo program. 
- Create a class design to represent a filesystem. 
- Design an OO representation to model HTML. 
- How do you print out the nodes of a tree in level-order (i.e. first level, then 2nd level, then 3rd level, etc.) 

Data structure questions:
What are some really common data structures, e.g. in java.util? 
Can you implement a Map with a tree? What about with a list? 
What's the worst-case insertion performance of a hashtable? Of a binary tree? O(1) unless resize in necessary for hastable; O(n^2) for binary tree
What are some options for implementing a priority queue? Can do either a normal queue where items are retrieved based on an extra key that defines
the priority level, or you can do a heap which is a binary tree where a parent node is always greater than all its child nodes

Talking through questions:

- Generally, what problem in OO development do design patterns solve? What's your favorite design pattern, and why?
- How does a binary tree work?

Big-O Notes
===========

O(1) - Determining if a number is even or odd; using a constant-size lookup table or hash table

O(logn) - Finding an item in a sorted array with a binary search (finding a name in a telephone book since it's sorted - binary search)

O(n) - Finding an item in an unsorted list; adding two n-digit numbers (finding a name in a telephone book iteratively given a phone number)

O(n^2) - Multiplying two n-digit numbers by a simple algorithm; adding two n×n matrices; bubble sort or insertion sort

O(n^3) - Multiplying two n×n matrices by simple algorithm

O(c^n) - Finding the (exact) solution to the traveling salesman problem using dynamic programming; determining if two logical statements are equivalent using brute force

O(n!) - Solving the traveling salesman problem via brute-force search

O(n^n) - Often used instead of O(n!) to derive simpler formulas for asymptotic complexity
