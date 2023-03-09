---
title: add_shape método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 260
url: /es/python-net/aspose.cells.drawing/shapecollection/add_shape/
is_root: false
---
##  add_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#MsoDrawingType-int-int-int-int-int-int}
Agrega una forma a la hoja de cálculo.


###  Devoluciones

Un objeto Forma.


```python
def add_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/es/python-net/aspose.cells.drawing/msodrawingtype) | Tipo de dibujo Mso.|
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de Shape desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int |Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de Shape desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de Shape, en unidades de píxel.|
| width | int | Representa el ancho de Shape, en unidades de píxel.|
###  Observaciones

El tipo no puede ser Gráfico/Comentario/Imagen/OleObject/Polygon/DialogBox
###  Ejemplo


```python
from aspose.cells.drawing import MsoDrawingType

# Add a shape of the specified type
shapeByType = shapes.add_shape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
