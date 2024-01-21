# CS260_Assignment_02 (Design)
# Eduarda (Duda) Reolon

There will not be any code implementation on this week's assignment!

1. Based on what we know about linked lists, stacks, and queues, design a queue data structure:

First, let's define what is a linked list, a stack, and a queue so that the concepts are clear before we design the code implementation.

Linked list: A linked list is a list that consists of nodes. Each node contains a data element and a pointer that points to the next node. 
![image](https://github.com/dudareolon/CS260_Assignment_02/assets/102680672/51fafbbd-a87c-47e1-85c3-6b020261afb0)
Figure 1.1

Stack: A stack is collection of elements that opperates in the Last In, First Out (LIFO) principle. Which means that the last element that was pushed into the stack will be the first element that will be popped out of the stack. Stacks can make use of pointers to indicate the bottom of the stack and the top of the stack.

![image](https://github.com/dudareolon/CS260_Assignment_02/assets/102680672/294ab757-fc1b-4c62-b328-028de4635516)

Figure 1.2

Queue: A queue is a linear data structure that does the opposite as the Stack. It is also a collection of elements but they opperate under the First In, First Out (FIFO) principle instead of opperating under the LIFO principle like the stack. First In, First Out means that the first element added to the queue is the first one to be removed. A queue can also make use of pointers to indicate the rear and the front of the queue. 

![image](https://github.com/dudareolon/CS260_Assignment_02/assets/102680672/aba1ab07-46a4-4f6f-a439-af2b7e8680e9)
Figure 1.3

1. Based on what we know about linked lists, stacks, and queues, design a queue data structure:

a) What functions are we likely to need for a queue to function like the one discussed in class?

The two main functions we need for the queue to function are:

  - Pop(): This function will remove the element that is in the front of the queue. To do this, the function will find the value that the front pointer is pointing to and assign this value to a variable that can be used outside of the function. The function will also reallocate the front pointer to point to the next node making this 'next node' the front of the queue. Lastly it will also decrease the size of the queue by one.

  - Push(Value): This function will insert the Value defined in the paranthesis at the rear of the queue. To do this, the function will allocate the variable Value to the slot pointed by the rear pointer, then it will increase the size of the queue by one and reallocate the rear pointer so that it will point to a new and empty node.

Although the two functions above are enough, to upgrade my code, I would also add these functions:

  - Size(): This functions returns the number of elements that are in the queue, in other words the size of the queue. Size will be variable that is started at 0, if the function pop is called the size decreases by one and if the function push is called the size increases by one.  
    
  - Empty(): This function runs a boolean relation that returns true in case the size of the queue is zero, meaning that it is empty. 
    
  - Front(): This function returns the value that the front pointer is pointing to, which would be the value removed from the queue if the pop function is called.  
    
  - Rear(): This function returns the value that the rear pointer is pointing to. This function is good to run as a test to make sure that the push function is working correctly. 
    

b) What values will we need to know about the structure for our queue to function properly?

  We would need to know the values that the rear and the front pointers are pointing to, but it would also be great to know the address of this values. If we know the address of the rear and the front values, then it is possible to use either the front or the rear pointer to move through the queue and print out all the values that are in the queue. We would need to know the size of the queue and have this variable be correctly updated every time the functions pop and push run. Lastly, we would also need to know if there is a capacity limit to the size of the queue so that we can update the function push to display an error message once the capacity is reached. 

2. Based on what we know about linked lists, design a list data structure that allows us to add (insert) or remove (delete) values at a given location in the list (instead of the top of a stack or the front or back of a queue):

  According to the reaserch I did, to have a linked list where you can add and remove values at any given location of the list, it is best to use a double-linked list instead of a linked list like the one described on Figure 1.1. That is because with a linked list you can only move forward, while with the double-linked list you can move through the values forward and backwards. A double-linked list looks like the image below:
  
![image](https://github.com/dudareolon/CS260_Assignment_02/assets/102680672/4a5ad5d9-241c-4b5d-ad2a-b61d79b3ea25)
Figure 1.4

a) What functions are we likely to need for a list to function like this?

b) What values will we need to know about the structure for our list to function properly?
