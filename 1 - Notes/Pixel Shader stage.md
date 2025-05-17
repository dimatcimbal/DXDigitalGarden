
2025-05-1706:41

Tags: [directx](directx.md) [programmable stage](programmable%20stage.md) [graphics pipeline](graphics%20pipeline.md)


The pixel shader is required to generate a color value output for each of the render target outputs bound to the pipeline. To accomplish this, it may sample textures or perform computations on the incoming fragment attributes. In addition, it can also override the depth value produced by the rasterizer stage, to allow for specialized algorithms to be implemented in the pixel shader stage.

After the pixel shader has finished its work, its output is passed to the output merger
stage.