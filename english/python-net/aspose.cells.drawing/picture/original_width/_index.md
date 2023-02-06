---
title: original_width property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 950
url: /python-net/aspose.cells.drawing/picture/original_width/
is_root: false
---

## original_width property


Gets the original width of the picture.

### Example 


```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Gets the original width of the picture.
picWidth = pic.original_width
# Save the excel file.
workbook.save("result.xlsx")

```
### Definition:
```python
@property
def original_width(self):
    ...
```

### See Also
* module [aspose.cells.drawing](../../)
* class [Picture](/cells/python-net/aspose.cells.drawing/picture)
