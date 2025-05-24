# Ex 5(E) Adjacency List Representation
## DATE: 22.04.2025
## AIM:
To write a C program to represent the given graph using the adjacency list.

## Algorithm

1.Start the program and declare necessary variables.

2.Read the number of vertices N and the number of edges n from the user.

3.Create an array of edges of size n.

4.Loop through the array to read each edge’s source and destination vertices.

5.Use the edges to create a graph by calling createGraph().

6.Print the adjacency list of the graph using printGraph().

7.End the program.

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: Shree Lekha.S
RegisterNumber: 212223110052
*/

int main(void)
{   int n,i;
    scanf("%d",&N);
    scanf("%d",&n);
    // input array containing edges of the graph (as per the above diagram)
    // (x, y) pair in the array represents an edge from x to y
    struct Edge edges[n];
    for (i = 0; i < n; i++)
    {
        // get the source and destination vertex
        scanf("%d",&edges[i].src);
        scanf("%d",&edges[i].dest);
      
    }
   
    // construct a graph from the given edges
    struct Graph *graph = createGraph(edges, n);
 
    // Function to print adjacency list representation of a graph
    printGraph(graph);
 
    return 0;
}
```

## Output:
![image](https://github.com/user-attachments/assets/5085a7dc-c0a1-4674-b2c2-aeb01ffbd2ed)


## Result:
Thus, the C program to represent the given graph using the adjacency list is implemented successfully
