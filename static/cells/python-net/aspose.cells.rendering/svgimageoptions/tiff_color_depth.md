##tiff_color_depth property
## tiff_color_depth property
Gets or sets bit depth to apply only when saving pages to the `Tiff` format.
### Remarks
Has effect only when saving to TIFF.
If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.
### Definition:
```python
@property
def tiff_color_depth(self):
...
@tiff_color_depth.setter
def tiff_color_depth(self, value):
...
```
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`ColorDepth`](/cells/python-net/aspose.cells.rendering/colordepth)
* class [`SvgImageOptions`](/cells/python-net/aspose.cells.rendering/svgimageoptions)
