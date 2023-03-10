---
title: add_oval método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 200
url: /es/python-net/aspose.cells.drawing/shapecollection/add_oval/
is_root: false
---
##  add_oval(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega un óvalo a la hoja de cálculo.


###  Devoluciones

Un objeto ovalado.


```python
def add_oval(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de Oval desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de Oval desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de Oval, en unidades de píxel.|
| width | int | Representa el ancho de Oval, en unidades de píxel.|

###  Ejemplo

```python

# add a oval
oval = shapes.add_oval(1, 0, 1, 0, 50, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
