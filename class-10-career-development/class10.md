401JS -- Linked Lists
================================

## Daily Plan

* Notes:
  * Final Whiteboard Exam
* Data Structures - Why?
* Review whiteboarding
* Linked Lists
  * Live-code: append/prepend
  * Whiteboarding
* Review Lab Assignment

## Abstract Data Type Resources
* Skim [ADT Wiki]

## Linked List Resources
* Watch [linked lists]
* Skim [linked list wiki]

# Learning Objectives
* The students will be able to implement a linked list
* The students will be able to implement a doubly linked list
* The students will be able to identify use cases for linked lists

# Overview
#### Singly Linked List
* There are no FILO/FIFO-style constraints on Lists.
* Singly linked lists contain nodes which have a data field as well as a 'next' field, which points to the next node in line of nodes.
* Operations that can be performed on singly linked lists include:
  * Insertion (Beginning, End, AfterNode(x), BeforeNode(x))
  * Deletion (Beginning, End, SpecificNode(x))
  * Traversal (Done from the head of the list)
* Singly Linked Lists can store both the Head and Tail pointers, though not a common implementation.

#### Doubly Linked List
* There are no FILO/FIFO-style constraints on Lists.
* Doubly linked lists contain nodes which have a data field as well as a 'next' AND 'prev' field, which points to the next and previous nodes in line of nodes.
* Operations that can be performed on singly linked lists include:
  * Insertion (Beginning, End, AfterNode(x), BeforeNode(x))
  * Deletion (Beginning, End, SpecificNode(x))
  * Traversal (Done from the head or the tail of the list)
* Doubly Linked Lists commonly store both the Head and Tail pointers.

#### Whiteboard Exercise (Group of 3)
* implement `reverse()` as a pure method
* (stretch) find the nth node from the end of the list (offsets)
* (stretch) find the middle of the list


[linked lists]: https://www.youtube.com/watch?v=njTh_OwMljA
[linked list wiki]: https://en.wikipedia.org/wiki/Linked_list
[ADT Wiki]: https://en.wikipedia.org/wiki/Abstract_data_type



## Final Exam: During weeks eight and nine or nine and ten, there will be a twenty minute technical interview. We will be given a whiteboard exam.


## Whiteboard Interview Process
1. Repeat the problem.
2. Questions/clarification
  - State assumptions
3. Review your thought process
  - 40,000 foot view
4. Pseudo-code
5. Assertions
6. Solution

## Questions
1. What kinds of questions might we be asked?
  - Given a string of words, what function can you use to generate a thousand words?
  - Implement a linked list.
  - Binary trees--traversal, how do we use code to find a node in a binary tree?
  - Solve this problem: Here's an input. What's the output?
  - Implement a data structure and use it for a real life problem.
2. How long does the whole process usually take?
  - Fizzbuzz and more!
  -
3. How do you react to a whiteboard problem that you have no idea how to solve?
  - Never just say, "I don't know."
  - Go back over the problem domain and ask questions. Clarify.
  - Often, the most important thing is how you work through the problem rather than whether you actually solve it.
  -
4. At some point, someone may pull up a site and ask, "How would you architect this site?"
  - Work through it one piece at a time.
  - Build out in verbal terms what the architecture might look like.
    + If you're on the phone, it may be all verbal, but if it's in person, there could be some whiteboarding.

**********************************************************************
## Stacks versus Queues
### Linked Lists
1. In a singly linked list, each node contains the value of the node and a link to the next node in the list.
  - A singly linked list as a data structure will keep track of just the node at the head of the list.
  - When we create this linked list and create a node, that node will be at the head of the list. When we create a new node, we prepend it--put it at the head of the list and move the first one back.
  - In a singly linked list, there is no tail.
2. Methods
  - Prepend: adds a new node to the head of the list
    + Creates a new node
    + Checks for a list
      - if empty, make new node
      - if not, attach to beginning of list, reassign new node to head of list, and make point to last old node.
  - Append:  
3. What is a node?
  - We're talking about abstract data structures
    + You are likely never going to sit down and code this thing out as an implementation to a solution.
    + You are going to adapt this data structure to a solution you are trying to create.
  - It's a way to structure data to be performant (hmmm).  
4.
5.
6.
