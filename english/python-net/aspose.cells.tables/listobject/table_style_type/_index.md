---
title: table_style_type property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 290
url: /python-net/aspose.cells.tables/listobject/table_style_type/
is_root: false
---

## table_style_type property


Gets and the built-in table style.

### Example 


```python
from aspose.cells import Workbook
from aspose.cells.tables import TableStyleType

workbook = Workbook("Book1.xlsx")
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.table_style_type = TableStyleType.TABLE_STYLE_DARK2
workbook.save("TableStyle.xlsx")

```

### See Also
* module [aspose.cells.tables](../../)
* class [ListObject](/cells/python-net/aspose.cells.tables/listobject)
