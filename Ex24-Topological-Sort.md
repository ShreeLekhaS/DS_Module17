# Ex 5(D) Topological Sort
## DATE:
## AIM:
To compose the code to determine whether the topological ordering for the following graph is possible or not.

![image](https://github.com/user-attachments/assets/c74a7111-9b59-475c-aad4-9baf23d50ec0)


## Algorithm

1.Start the program and create the graph.

2.Calculate indegree for all vertices.

3.Enqueue vertices with indegree 0.

4.While queue not empty, dequeue a vertex, add it to the topological order, remove its outgoing edges updating indegrees, and enqueue any vertices whose indegree becomes zero.

5.If all vertices processed, print topological order; else, report cycle.

6.End the program.

## Program:
```
/*
Program to determine whether the topological ordering for the following graph is possible or not
Developed by: Shree Lekha.S
RegisterNumber: 212223110052
*/

int main()
{
        int i,v,count,topo_order[MAX],indeg[MAX];

        create_graph();

        /*Find the indegree of each vertex*/
        for(i=0;i<n;i++)
        {
                indeg[i] = indegree(i);
                if( indeg[i] == 0 )
                        insert_queue(i);
        }

        count = 0;

        while(  !isEmpty_queue( ) && count < n )
        {
                v = delete_queue();
        topo_order[++count] = v; /*Add vertex v to topo_order array*/
                /*Delete all edges going from vertex v */
                for(i=0; i<n; i++)
                {
                        if(adj[v][i] == 1)
                        {
                                adj[v][i] = 0;
                                indeg[i] = indeg[i]-1;
                                if(indeg[i] == 0)
                                        insert_queue(i);
                        }
                }
        }

        if( count < n )
        {
                printf("No topological ordering possible, graph contains cycle\n");
                exit(1);
        }
        printf("Vertices in topological order are :\n");
        for(i=1; i<=count; i++)
                printf( "%d ",topo_order[i] );
        printf("\n");

        return 0;
}

```

## Output:



## Result:
Thus, the C program for determining whether the topological ordering for the following graph is possible or not, is implemented successfully.
