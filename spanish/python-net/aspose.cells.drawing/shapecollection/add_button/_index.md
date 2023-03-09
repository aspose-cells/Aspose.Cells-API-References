---
title: add_button método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 60
url: /es/python-net/aspose.cells.drawing/shapecollection/add_button/
is_root: false
---
##  add_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega un botón a la hoja de trabajo.


###  Devoluciones

Un objeto Botón.


```python
def add_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de Button desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de Button desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de Button, en unidades de píxel.|
| width | int | Representa el ancho de Button, en unidades de píxel.|

###  Ejemplos

```python

# add a button
button = shapes.add_button(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
