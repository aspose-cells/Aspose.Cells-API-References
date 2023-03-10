---
title: table_style_type propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 290
url: /es/python-net/aspose.cells.tables/listobject/table_style_type/
is_root: false
---
##  table_style_type propiedad

Obtiene y el estilo de tabla integrado.

###  Ejemplo

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
###  Definición:
```python
@property
def table_style_type(self):
    ...
@table_style_type.setter
def table_style_type(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.tables](../../)
* clase [ListObject](/cells/es/python-net/aspose.cells.tables/listobject)
* clase [TableStyleType](/cells/es/python-net/aspose.cells.tables/tablestyletype)
