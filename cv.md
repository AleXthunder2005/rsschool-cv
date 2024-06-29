# Aleksandr Narivonchik
## Contact information:
#### **E-mail:** aleksandrnar2005@gmail.com  
#### **Telegram:** @AleXthunder_18  
## Briefly About Myself:
#### I'm Aleksandr and i'm 18. I study at Belarusian State University of Informatics and Radioelectronics (BSUIR). In my opinion, a job of Software Developer is the very interest, so I want to learn a lot of technology to be able to do as much as possible.
## Skills:
* Java
* Git/GitHub
* Figma
## Code example:
#### Task: *Find the minimum path between two vertices of the graph using the Ford-Bellman algorithm:*
```
    private static int findMinWay(ArrayList<Integer>[] incidentLists, Edge[] edges, int src, int dest) {
        int n = incidentLists.length;
 
        int[] dist = new int[n];
        for(int i = 0; i < n; i++){
            dist[i] = Integer.MAX_VALUE;
        }
        dist[src-1] = 0;
 
        for (int i = 0; i < n-1; i++){
            for (int j = 0; j < edges.length; j++){
                if ((dist[edges[j].src - 1] != Integer.MAX_VALUE) && (dist[edges[j].src - 1] + edges[j].weight < dist[edges[j].dest - 1]))
                    dist[edges[j].dest - 1] = dist[edges[j].src - 1] + edges[j].weight;
            }
        }
        if (dist[dest-1] == Integer.MAX_VALUE)
            return -1;
        else
            return dist[dest-1];
    }
```
## Education:
#### First-year student of BSUIR
## Languages:
#### English: ***Pre-Intermediate***
