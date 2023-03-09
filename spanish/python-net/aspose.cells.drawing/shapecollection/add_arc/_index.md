---
title: add_arc método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells.drawing/shapecollection/add_arc/
is_root: false
---
##  add_arc(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega un ArcShape a la hoja de trabajo.


###  Devoluciones

Un objeto ArcShape.


```python
def add_arc(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de ArcShape desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de ArcShape desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de ArcShape, en unidades de píxel.|
| width | int |Representa el ancho de ArcShape, en unidades de píxel.|

###  Ejemplos

```python

# add a arc
arcShape = shapes.add_arc(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
