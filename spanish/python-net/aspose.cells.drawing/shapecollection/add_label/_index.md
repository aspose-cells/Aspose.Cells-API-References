---
title: add_label método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 130
url: /es/python-net/aspose.cells.drawing/shapecollection/add_label/
is_root: false
---
##  add_label(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega una etiqueta a la hoja de cálculo.


###  Devoluciones

Un objeto de etiqueta.


```python
def add_label(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de la etiqueta desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de la etiqueta desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de la etiqueta, en unidades de píxel.|
| width | int | Representa el ancho de la etiqueta, en unidades de píxel.|

###  Ejemplos

```python

# add a label
label = shapes.add_label(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
