---
title: copy method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/range/copy/
is_root: false
---

## copy(range) {#Range}

Copies data (including formulas), formatting, drawing objects etc. from a source range.



```python
def copy(self, range):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| range | [Range](/cells/python-net/aspose.cells/range) | Source [Range](/cells/python-net/aspose.cells/range) object. |

### Example 


```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A6:A10")
# Copy the range.
range1.copy(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```


## copy(range, options) {#Range-PasteOptions}

Copying the range with paste special options.



```python
def copy(self, range, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| range | [Range](/cells/python-net/aspose.cells/range) | The source range. |
| options | [PasteOptions](/cells/python-net/aspose.cells/pasteoptions) | The paste special options. |



### See Also
* module [aspose.cells](../../)
* class [Range](/cells/python-net/aspose.cells/range)
