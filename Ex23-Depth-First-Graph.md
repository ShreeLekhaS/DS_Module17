# Ex 5(C) Depth First Graph
## DATE:
## AIM:
To compose the code for the function createNode to traverse the graph below in the depth first fashion.

![image](https://github.com/user-attachments/assets/63552824-d0a3-49c6-a473-6db27d1f03e4)

## Algorithm

1.Start the program and define a structure for a graph node with a vertex value and a pointer to the next node.

2.Create a function createNode that takes an integer vertex v as input.

3.Inside the function, allocate memory dynamically for a new node.

4.Initialize the node’s vertex field with the input v.

5.Set the next pointer of the node to NULL (since it’s a standalone node initially).

6.Return the newly created node to be used in the adjacency list.   

## Program:
```
/*
Program to traverse the graph below in the depth first fashion
Developed by: Shree Lekha.S
RegisterNumber: 212223110052
*/

/*#include<stdio.h>
#include <stdlib.h>
structnode
{
  int vertex;
  struct node* next;
};
struct node*createNode(int v);
struct Graph
{
  intnumVertices;
  int* visited;
  // We need int**to storeatwodimensionalarray.
  // Similary, we needstruct node**to storeanarrayofLinked lists
  struct node** adjLists;
};*/
struct node*createNode(int v)
{
  structnode* newNode=malloc(sizeof(struct node));
  newNode->vertex=v;
  newNode->next=NULL;
  returnnewNode;
}
```

## Output:

![image](https://github.com/user-attachments/assets/12da1043-24ae-4b1f-b6e3-976aea5250b1)


## Result:
Thus, the C code for the function createNode to traverse the graph below in the depth first fashion is implemented successfully
