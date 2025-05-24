# Ex 5(A) Representation of Graph
## DATE: 11.04.2025
## AIM:
To write a C program to display the adjacency matrix of the given graph by supplying the edges and the number of vertices.

## Algorithm

1.Start the program and read the number of vertices V.

2.Initialize a V x V adjacency matrix with all zeros.

3.Calculate the maximum number of edges me in an undirected graph as V*(V-1)/2.

4.Loop to read pairs of vertices (e1, e2) representing edges until -1 -1 is entered or max edges are reached.

5.For each valid edge, update the adjacency matrix by marking the presence of an edge between e1 and e2.

6.Print the final adjacency matrix to show the graph’s connections and end the program.  

## Program:
```
/*
Program to display the adjacency matrix of the given graph
Developed by: Shree Lekha.S
RegisterNumber: 212223110052 
*/

/*#include<stdio.h> 
int V; 
 
//init matrix to 0 
void init(int arr[][V]) 
{ 
int i,j; 
for(i = 0; i < V; i++) 
for(j = 0; j < V; j++) 
arr[i][j] = 0; 
} 
*/ 
int main() 
{ int e1,e2,me,n,i; 
scanf("%d",&V); 
int adjMatrix[V][V]; 
init(adjMatrix); 
n=V; 
me=n*(n-1)/2; 
for(i=0;i<me;i++) 
{ 
scanf("%d%d",&e1,&e2); 
addEdge(adjMatrix,e1,e2); 
if(e1==-1 && e2==-1) 
{ 
break; 
} 
} 
printAdjMatrix(adjMatrix); 
 
}

```

## Output:

![image](https://github.com/user-attachments/assets/f1bf4d23-b8f8-4e3e-b60e-37729dbc035b)


## Result:
Thus, the C program to print the adjacency matrix of the given graph is implemented successfully.
