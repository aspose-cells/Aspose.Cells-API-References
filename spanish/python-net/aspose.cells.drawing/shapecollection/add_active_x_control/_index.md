---
title: add_active_x_control método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.drawing/shapecollection/add_active_x_control/
is_root: false
---
##  add_active_x_control(type, top_row, top, left_column, left, width, height) {#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int}
Crea un Control Activex.


###  Devoluciones




```python
def add_active_x_control(self, type, top_row, top, left_column, left, width, height):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| type | aspose.cells.drawing.activexcontrols.ControlType | El tipo de control.|
| top_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de Shape desde su fila izquierda, en unidades de píxel.|
| left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de Shape desde su columna izquierda, en unidades de píxel.|
| width | int | Representa el ancho de Forma, en unidades de píxeles.|
| height | int | Representa la altura de Shape, en unidades de píxeles.|

###  Ejemplos

```python
from aspose.cells.drawing.activexcontrols import ControlType

# add an ActiveX control
activeXControl = shapes.add_active_x_control(ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
