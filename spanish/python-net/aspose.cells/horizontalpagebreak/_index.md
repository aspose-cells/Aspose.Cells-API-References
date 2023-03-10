---
title: HorizontalPageBreak clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 750
url: /es/python-net/aspose.cells/horizontalpagebreak/
is_root: false
---
##  HorizontalPageBreak clase
Encapsula el objeto que representa un salto de página horizontal.



El tipo HorizontalPageBreak expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [start_column](/cells/es/python-net/aspose.cells/horizontalpagebreak/start_column) | Obtiene el índice de la columna inicial de este salto de página horizontal.|
| [end_column](/cells/es/python-net/aspose.cells/horizontalpagebreak/end_column) | Obtiene el índice de la columna final de este salto de página horizontal.|
| [row](/cells/es/python-net/aspose.cells/horizontalpagebreak/row) | Obtiene el índice de fila basado en cero.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Add a page break at cell Y30
Index = worksheet.horizontal_page_breaks.add("Y30")
# get the newly added horizontal page break
hPageBreak = worksheet.horizontal_page_breaks[Index]

```

###  Ver también
* módulo [aspose.cells](..)
