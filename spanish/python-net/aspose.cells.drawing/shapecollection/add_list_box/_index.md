---
title: add_list_box método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 170
url: /es/python-net/aspose.cells.drawing/shapecollection/add_list_box/
is_root: false
---
##  add_list_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega un ListBox a la hoja de trabajo.


###  Devoluciones

Un objeto ListBox.


```python
def add_list_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de ListBox desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de ListBox desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de ListBox, en unidades de píxel.|
| width | int | Representa el ancho de ListBox, en unidades de píxel.|

###  Ejemplo

```python

# add a list box
listBox = shapes.add_list_box(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
