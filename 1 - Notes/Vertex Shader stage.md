
2025-05-1706:31

Tags: [directx](directx.md) [programmable stage](programmable%20stage.md) [graphics pipeline](graphics%20pipeline.md)


The vertex shader stage reads the assembled vertex data from the input assembler
stage and processes a single vertex at a time. This is the first programmable stage in the pipeline, and it applies the current vertex shader program to each input vertex. It cannot create or destroy vertices; it can only process the vertices that are given to it. In addition, every vertex is processed in isolation—the information from one vertex shader invocation is never accessible in another invocation. The primary responsibility of the vertex shader used to be to project the vertex positions into clip space. In general, any operation that must be performed on every vertex of the input model should be performed in the vertex shader.