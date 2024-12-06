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
    ![Uploading image.png…]()
