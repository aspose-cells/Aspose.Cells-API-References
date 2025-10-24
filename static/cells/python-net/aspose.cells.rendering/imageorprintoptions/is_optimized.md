##is_optimized property
## is_optimized property
Indicates whether to optimize the output elements.
### Remarks
Default value is false.
Currently when this property is set to true, the following optimizations will be done:
1. optimize the border lines.
2. optimize the file size while rendering to Svg image.
### Definition:
```python
@property
def is_optimized(self):
...
@is_optimized.setter
def is_optimized(self, value):
...
```
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`ImageOrPrintOptions`](/cells/python-net/aspose.cells.rendering/imageorprintoptions)
