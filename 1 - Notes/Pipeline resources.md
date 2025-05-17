
2025-05-1807:10

Tags: [directx](directx.md) [graphics pipeline](graphics%20pipeline.md)

Resources:
* [Buffers](Buffers.md)
* [Textures](Textures.md)

In general, there are two different domains for using resources—one is from C/C++, and the other is from HLSL. 
* C/C++ is primarily concerned with creating resources and binding/unbinding them to the desired locations. 
* HLSL is more concerned with actually manipulating and using the contents of the resources. 

A resource must be bound to the pipeline in order to be used. When a resource is
bound to the pipeline, it can be used as a data input, an output, or both. This primarily depends on where and how it is bound to the pipeline. For example, a vertex buffer bound as an input to the input assembler is clearly an input, and a 2D texture bound to the output merger stage as a render target is clearly an output. However, what if we wanted to use the contents of the output render target in a subsequent rendering pass? It could also be bound to a pixel shader as a texture resource to be sampled during the next rendering operation.

To help the runtime (and the developer!) determine the intended use of a resource,
the API provides the concept of *resource views*. When a particular resource can be bound to the pipeline in several different types of locations in the pipeline, it must be bound with a resource view that specifies how it will be used. 

Resource views:
* *render target* view
* *depth stencil* view
* *shader resource* view
* *unordered access* view

Both render target and depth stencil views are used for binding render and depth targets to the pipeline, respectively.

Shader resource view allows for resources to be bound for reading in any of the programmable shader stages.

Unordered access view allows a resource to be bound for simultaneous random read and write access, but is only available for use in the [Compute Shader stage](Compute%20Shader%20stage.md) and [Pixel Shader stage](Pixel%20Shader%20stage.md).

Resource binding types not requiring a resource view
* Vertex buffer
* Index buffer
* Constant buffer