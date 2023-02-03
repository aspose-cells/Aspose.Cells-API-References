---
title: to_tiff method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 60
url: /python-net/aspose.cells.rendering/sheetrender/to_tiff/
is_root: false
---

## to_tiff(stream) {#io.RawIOBase}

Render whole worksheet as Tiff Image to stream.



```python
def to_tiff(self, stream):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | the stream of the output image |


## to_tiff(filename) {#str}

Render whole worksheet as Tiff Image to a file.



```python
def to_tiff(self, filename):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| filename | str | the filename of the output image |

### Example 


The following code outputs all the pages of the first sheet to Tiff image.

```python
from aspose.cells import SaveFormat, Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

# load the source file with images.
wb = Workbook("Book1.xlsx")
imgOpt = ImageOrPrintOptions()
# set output image type.
imgOpt.save_format = SaveFormat.TIFF
# render the first sheet.
sr = SheetRender(wb.worksheets[0], imgOpt)
# output all the pages of the sheet to Tiff image.
sr.to_tiff("output.tiff")

```



### See Also
* module [aspose.cells.rendering](../../)
* class [SheetRender](/cells/python-net/aspose.cells.rendering/sheetrender)
