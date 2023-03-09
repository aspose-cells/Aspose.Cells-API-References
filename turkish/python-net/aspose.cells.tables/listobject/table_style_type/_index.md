---
title: table_style_type mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 290
url: /tr/python-net/aspose.cells.tables/listobject/table_style_type/
is_root: false
---
##  table_style_type mülk

Alır ve yerleşik tablo stili.

###  örnekler

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
###  Tanım:
```python
@property
def table_style_type(self):
    ...
@table_style_type.setter
def table_style_type(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.tables](../../)
* sınıf [ListObject](/cells/tr/python-net/aspose.cells.tables/listobject)
* sınıf [TableStyleType](/cells/tr/python-net/aspose.cells.tables/tablestyletype)
