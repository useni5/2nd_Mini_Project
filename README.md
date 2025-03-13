Memory Leak Risk: Memory is only freed upon exiting (case 8). If the program terminates unexpectedly, it could lead to a memory leak. A freeQueue() function would help.

Inefficient Dequeue (pop) Operation: The queue shifts front forward, and eventually, even if space is available, new elements cannot be added.
Solution: Implement a circular queue to reuse space efficiently.


Example 1: Normal Operations
Input:
mathematica
Copy
Edit
Enter the capacity of the queue: 5

Menu:
1. Enqueue (Push)
2. Dequeue (Pop)
3. Peek
4. Size
5. Is Empty
6. Is Full
7. Print Elements
8. Exit
Enter your choice: 1
Enter value to enqueue: 10

Enter your choice: 1
Enter value to enqueue: 20

Enter your choice: 1
Enter value to enqueue: 30

Enter your choice: 7
Output:
yaml
Copy
Edit
Enqueued element: 10
Enqueued element: 20
Enqueued element: 30
Queue elements: 10 20 30
