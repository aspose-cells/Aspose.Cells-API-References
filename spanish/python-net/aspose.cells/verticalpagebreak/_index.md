---
title: VerticalPageBreak clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1560
url: /es/python-net/aspose.cells/verticalpagebreak/
is_root: false
---
##  VerticalPageBreak clase
Encapsula el objeto que representa un salto de página vertical.



El tipo VerticalPageBreak expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [start_row](/cells/es/python-net/aspose.cells/verticalpagebreak/start_row) | Obtiene el índice de la fila inicial del salto de página vertical.|
| [end_row](/cells/es/python-net/aspose.cells/verticalpagebreak/end_row) | Obtiene el índice de fila final del salto de página vertical.|
| [column](/cells/es/python-net/aspose.cells/verticalpagebreak/column) | Obtiene el índice de columna del salto de página vertical.|



###  Ejemplo

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Ver también
* módulo [aspose.cells](..)
