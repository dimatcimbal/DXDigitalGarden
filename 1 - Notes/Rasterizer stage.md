
2025-05-1706:38

Tags: [directx](directx.md)  [fixed-function stage](fixed-function%20stage.md) [graphics pipeline](graphics%20pipeline.md)


The rasterizer produces [Fragmet](Fragmet.md)s from the geometric data passed to it, by determining which pixels of a render target are covered by the geometry. Each fragment receives interpolated versions of all of the per-vertex attributes, to provide the information needed for further processing later in the pipeline. In addition, the rasterizer produces a depth value for each fragment, which will later be used for visibility testing in the output merger stage.

Once a fragment has been generated, the [Pixel Shader stage](Pixel%20Shader%20stage.md) is invoked to process it.
