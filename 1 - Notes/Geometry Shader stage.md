
2025-05-1706:34

Tags: [directx](directx.md) [programmable stage](programmable%20stage.md) [graphics pipeline](graphics%20pipeline.md)


The geometry shader operates on a geometric level. In practice, this means that it operates on complete geometric primitives, and also produces geometric primitives. This stage can both add and remove data elements from the pipeline, which allows for some interesting, non-traditional uses. In addition, it can take one type of geometry as input and generate a different type of geometry as output. This allows the conversion of single vertices into complete triangles, or even multiple triangles. The geometry shader is also the conduit through which processed geometry can be streamed out of the pipeline into a buffer resource. This is accomplished in the stream output stage.