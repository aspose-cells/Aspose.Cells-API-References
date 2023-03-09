---
title: add_spinner método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 290
url: /es/python-net/aspose.cells.drawing/shapecollection/add_spinner/
is_root: false
---
##  add_spinner(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega un Spinner a la hoja de trabajo.


###  Devoluciones

Un objeto Spinner.


```python
def add_spinner(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int |Representa el desplazamiento vertical de Spinner desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de Spinner desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de Spinner, en unidades de píxel.|
| width | int | Representa el ancho de Spinner, en unidades de píxel.|

###  Ejemplos

```python

# add a spinner
spinner = shapes.add_spinner(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
