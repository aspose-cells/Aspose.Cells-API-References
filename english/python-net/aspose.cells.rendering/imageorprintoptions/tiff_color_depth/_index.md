---
title: tiff_color_depth property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 340
url: /python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth/
is_root: false
---

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
* module [aspose.cells.rendering](../../)
* class [ColorDepth](/cells/python-net/aspose.cells.rendering/colordepth)
* class [ImageOrPrintOptions](/cells/python-net/aspose.cells.rendering/imageorprintoptions)
