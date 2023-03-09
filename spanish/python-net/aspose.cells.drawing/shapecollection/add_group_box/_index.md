---
title: add_group_box método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 110
url: /es/python-net/aspose.cells.drawing/shapecollection/add_group_box/
is_root: false
---
##  add_group_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega un GroupBox a la hoja de cálculo.


###  Devoluciones

Un objeto GroupBox.


```python
def add_group_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de GroupBox desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de GroupBox desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de GroupBox, en unidades de píxel.|
| width | int | Representa el ancho de GroupBox, en unidades de píxel.|

###  Ejemplos

```python

# add a group box
groupBox = shapes.add_group_box(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
