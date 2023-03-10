---
title: add_line método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 150
url: /es/python-net/aspose.cells.drawing/shapecollection/add_line/
is_root: false
---
##  add_line(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega un LineShape a la hoja de cálculo.


###  Devoluciones

Un objeto LineShape.


```python
def add_line(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de LineShape desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de LineShape desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de LineShape, en unidades de píxel.|
| width | int | Representa el ancho de LineShape, en unidades de píxel.|

###  Ejemplo

```python

#  add a line object
lineShape = shapes.add_line(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
