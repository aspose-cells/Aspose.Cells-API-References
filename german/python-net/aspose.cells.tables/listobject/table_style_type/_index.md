---
title: table_style_type Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 290
url: /de/python-net/aspose.cells.tables/listobject/table_style_type/
is_root: false
---
##  table_style_type Eigentum

Ruft und den integrierten Tabellenstil ab.

###  Beispiele

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
###  Definition:
```python
@property
def table_style_type(self):
    ...
@table_style_type.setter
def table_style_type(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.tables](../../)
* Klasse [ListObject](/cells/de/python-net/aspose.cells.tables/listobject)
* Klasse [TableStyleType](/cells/de/python-net/aspose.cells.tables/tablestyletype)
