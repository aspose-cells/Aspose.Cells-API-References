---
title: html_text property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 480
url: /python-net/aspose.cells.drawing/cellsdrawing/html_text/
is_root: false
---

## html_text property


Gets and sets the html string which contains data and some formats in this textbox.

### Example 


```python

html = shape.html_text
if html == null  || html == "":
    shape.html_text = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"

```
### Definition:
```python
@property
def html_text(self):
    ...
@html_text.setter
def html_text(self, value):
    ...
```

### See Also
* module [aspose.cells.drawing](../../)
* class [CellsDrawing](/cells/python-net/aspose.cells.drawing/cellsdrawing)
