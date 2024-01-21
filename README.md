# CS260_Assignment_02 (Design)
# Eduarda (Duda) Reolon

There will not be any code implementation on this week's assignment!

1. Based on what we know about linked lists, stacks, and queues, design a queue data structure:

First, let's define what is a linked list, a stack, and a queue so that the concepts are clear before we design the code implementation.

Linked list: A linked list is a list that consists of nodes. Each node contains a data element and a pointer that points to the next node. 
![image](https://github.com/dudareolon/CS260_Assignment_02/assets/102680672/51fafbbd-a87c-47e1-85c3-6b020261afb0)

Stack: A stack is collection of elements that opperates in the Last In, First Out (LIFO) principle. Which means that the last element that was pushed into the stack will be the first element that will be popped out of the stack. Stacks can make use of pointers to indicate the bottom of the stack and the top of the stack.

![image](https://github.com/dudareolon/CS260_Assignment_02/assets/102680672/294ab757-fc1b-4c62-b328-028de4635516)

Queue: A queue is a linear data structure that does the opposite as the Stack. It is also a collection of elements but they opperate under the First In, First Out (FIFO) principle instead of opperating under the LIFO principle like the stack. First In, First Out means that the first element added to the queue is the first one to be removed. A queue can also make use of pointers to indicate the rear and the front of the queue. 

![image](https://github.com/dudareolon/CS260_Assignment_02/assets/102680672/aba1ab07-46a4-4f6f-a439-af2b7e8680e9)

1. Based on what we know about linked lists, stacks, and queues, design a queue data structure:
a) What functions are we likely to need for a queue to function like the one discussed in class?
The two main functions we need for the queue to function are:
  - Pop():
  - Push(Value):
Although the two functions above are enough, to upgrade my code, I would also add these functions:
  - Size():
  - Empty():
  - Front():
  - Rear():

b) What values will we need to know about the structure for our queue to function properly?

2. Based on what we know about linked lists, design a list data structure that allows us to add (insert) or remove (delete) values at a given location in the list (instead of the top of a stack or the front or back of a queue):
  - What functions are we likely to need for a list to function like this?
  - What values will we need to know about the structure for our list to function properly?**
