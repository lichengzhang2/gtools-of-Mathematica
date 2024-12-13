```
glist = Import["!geng 7 -t -C", "Graph6"];
Grid[Partition[
  Table[Labeled[
    Graph[glist[[i]], GraphLayout -> "CircularEmbedding", 
     PlotTheme -> "Monochrome", VertexSize -> .17 {1, 1}, 
     ImageSize -> {50, 50}, VertexStyle -> GrayLevel[.6]], 
    Style[i, FontFamily -> "Baskerville"], Bottom], {i, 
    Length[glist]}], UpTo[10]], Frame -> All]
```


![image](https://github.com/user-attachments/assets/be002fdf-1d45-447d-a74f-094793016eef)

2. Function: rotateGraph

```
 rotateGraph[g, 45 Degree]
```
![image](https://github.com/user-attachments/assets/c940e0d2-b93a-4f56-8311-49bcd632e1fc)
