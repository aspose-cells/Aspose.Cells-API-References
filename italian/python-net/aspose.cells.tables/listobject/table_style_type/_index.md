---
title: table_style_type proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 290
url: /it/python-net/aspose.cells.tables/listobject/table_style_type/
is_root: false
---
##  table_style_type proprietà

Ottiene e lo stile di tabella predefinito.

###  Esempio

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
###  Definizione:
```python
@property
def table_style_type(self):
    ...
@table_style_type.setter
def table_style_type(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.tables](../../)
* classe [ListObject](/cells/it/python-net/aspose.cells.tables/listobject)
* classe [TableStyleType](/cells/it/python-net/aspose.cells.tables/tablestyletype)
