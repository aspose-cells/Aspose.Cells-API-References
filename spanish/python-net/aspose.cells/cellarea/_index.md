---
title: CellArea clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 150
url: /es/python-net/aspose.cells/cellarea/
is_root: false
---
##  CellArea clase
Representa un área de celdas.



El tipo CellArea expone los siguientes miembros:

###  Constructores
| Constructor| Descripción|
| :- | :- |
| [CellArea()](/cells/es/python-net/aspose.cells/cellarea/__init__/#) | Construye una nueva instancia de CellArea|


###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [start_row](/cells/es/python-net/aspose.cells/cellarea/start_row) | Obtiene o establece la fila inicial de esta área.|
| [end_row](/cells/es/python-net/aspose.cells/cellarea/end_row) | Obtiene o establece la última fila de esta área.|
| [start_column](/cells/es/python-net/aspose.cells/cellarea/start_column) |Obtiene o establece la columna de inicio de esta área.|
| [end_column](/cells/es/python-net/aspose.cells/cellarea/end_column) | Obtiene o establece la columna final de esta área.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [create_cell_area(start_row, start_column, end_row, end_column)](/cells/es/python-net/aspose.cells/cellarea/create_cell_area/#int-int-int-int) | Crea un área de celda.|
| [create_cell_area(start_cell_name, end_cell_name)](/cells/es/python-net/aspose.cells/cellarea/create_cell_area/#str-str) | Crea un área de celda.|
| [compare_to(obj)](/cells/es/python-net/aspose.cells/cellarea/compare_to/#any) | Compare dos objetos CellArea según su esquina superior izquierda.|



###  Ejemplo

```python
from aspose.cells import CellArea

# Create Cell Area
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0

```

###  Ver también
* módulo [aspose.cells](..)
