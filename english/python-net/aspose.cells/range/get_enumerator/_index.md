---
title: get_enumerator method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 90
url: /python-net/aspose.cells/range/get_enumerator/
is_root: false
---

## get_enumerator() {#}

Gets the enumerator for cells in this Range.


### Returns 


The cells enumerator


```python
def get_enumerator(self):
    ...
```


### Remarks

When traversing elements by the returned Enumerator, the cells collection
should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted).
Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).
### Example 


```python
from aspose.cells import Workbook

workbook = Workbook("template.xlsx")
cells = workbook.worksheets[0].cells
en = cells.create_range("B2:C3").get_enumerator()
for cell in en:
    print(cell.name + ": "  + str(cell.value))

```



### See Also
* module [aspose.cells](../../)
* class [Range](/cells/python-net/aspose.cells/range)
