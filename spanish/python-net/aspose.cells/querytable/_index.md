---
title: QueryTable clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1230
url: /es/python-net/aspose.cells/querytable/
is_root: false
---
##  QueryTable clase
Representa QueryTable información.



El tipo QueryTable expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [connection_id](/cells/es/python-net/aspose.cells/querytable/connection_id) |Obtiene el identificador de conexión de la tabla de consulta.|
| [external_connection](/cells/es/python-net/aspose.cells/querytable/external_connection) | Obtiene la conexión externa relacionada.|
| [name](/cells/es/python-net/aspose.cells/querytable/name) | Obtiene el nombre de la tabla de consulta.|
| [result_range](/cells/es/python-net/aspose.cells/querytable/result_range) | Obtiene el rango del resultado.|
| [preserve_formatting](/cells/es/python-net/aspose.cells/querytable/preserve_formatting) | Devuelve o establece el PreserveFormatting del objeto.|
| [adjust_column_width](/cells/es/python-net/aspose.cells/querytable/adjust_column_width) | Devuelve o establece el AdjustColumnWidth del objeto.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Getting the first query table in the worksheet
qt = worksheet.query_tables[0]
# Getting display address of the query table.
address = qt.result_range.address

```

###  Ver también
* módulo [aspose.cells](..)
