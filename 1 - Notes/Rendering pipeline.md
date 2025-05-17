
2025-05-1706:21

Tags:  [directx](directx.md) [graphics pipeline](graphics%20pipeline.md) 


The rendering pipeline is intended to take a set of 3D object descriptions and convert
it into an image format that is suitable for presentation in the output window of an application.

![](../3%20-%20Resources/Pasted%20image%2020250517062443.png)
		J. Zink, M. Pettineo, J. Hoxley. Practical Rendering & Computation with DIrect3D11.

Stages
* [Input Assembler stage](Input%20Assembler%20stage.md)
* [Vertex Shader stage](Vertex%20Shader%20stage.md)
* Tessellation stages
	* Hull Shader stage
	* Tessellator
	* Domain shader stage
* [Geometry Shader stage](Geometry%20Shader%20stage.md)
* [Rasterizer stage](Rasterizer%20stage.md)
* [Pixel Shader stage](Pixel%20Shader%20stage.md)
* [Output Merger stage](Output%20Merger%20stage.md)