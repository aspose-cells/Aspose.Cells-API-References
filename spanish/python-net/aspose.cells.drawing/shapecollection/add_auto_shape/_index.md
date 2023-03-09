---
title: add_auto_shape método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/
is_root: false
---
##  add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#AutoShapeType-int-int-int-int-int-int}
Agrega una autoforma a la hoja de trabajo.


###  Devoluciones

Un objeto Forma.


```python
def add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| type | [AutoShapeType](/cells/es/python-net/aspose.cells.drawing/autoshapetype) | Tipo de forma automática.|
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de Shape desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de Shape desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de Shape, en unidades de píxeles.|
| width | int | Representa el ancho de Forma, en unidades de píxeles.|
###  Observaciones

El tipo no puede ser Gráfico/Comentario/Imagen/OleObject/Polygon/DialogBox
###  Ejemplos


```python
from aspose.cells.drawing import AutoShapeType

# Adds a AutoShape to the worksheet.
autoShape = shapes.add_auto_shape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
