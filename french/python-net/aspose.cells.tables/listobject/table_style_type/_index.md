---
title: table_style_type propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 290
url: /fr/python-net/aspose.cells.tables/listobject/table_style_type/
is_root: false
---
##  table_style_type propriété

Gets et le style de tableau intégré.

###  Exemple

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
###  Définition:
```python
@property
def table_style_type(self):
    ...
@table_style_type.setter
def table_style_type(self, value):
    ...
```

###  Voir également
* module [aspose.cells.tables](../../)
* classe [ListObject](/cells/fr/python-net/aspose.cells.tables/listobject)
* classe [TableStyleType](/cells/fr/python-net/aspose.cells.tables/tablestyletype)
