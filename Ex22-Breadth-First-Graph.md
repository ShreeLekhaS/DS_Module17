# Ex22 Breadth First Graph
## DATE:
## AIM:
To write a printQueue C function of the given graph that is to be traversed in the breadth first manner.

![image](https://github.com/user-attachments/assets/f483f48c-6af0-4027-a993-01c108a50933)


## Algorithm

1.Start the function and get the front index of the queue.

2.Check if the queue is empty using isEmpty().

3.If empty, print a message indicating the queue is empty.

4.If not empty, loop from the front index to the rear index of the queue.

5.Print each element in the queue during the loop, then end the function.

## Program:
```
/*
Program to traverse graph using BFS
Developed by: Shree Lekha.S
RegisterNumber: 212223110052
*/
void printQueue(struct queue* q) {
  int i = q->front;
 
  if (isEmpty(q)) {
    printf("Queue is empty");
  } else { 
    printf("Queue contains ");
    for (i = q->front; i < q->rear + 1; i++) {
      printf("%d ", q->items[i]);
    }
   }
}
```

## Output:
![image](https://github.com/user-attachments/assets/fa76e3a8-431d-4e43-8fcb-6d4922c85e50)

## Result:
Thus, the code for the printQueue function of the following graph that is to be traversed in the breadth first manner is implemented successfully.
