---
title: add_check_box método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells.drawing/shapecollection/add_check_box/
is_root: false
---
##  add_check_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega una casilla de verificación a la hoja de cálculo.


###  Devoluciones

El nuevo índice de objetos CheckBox.


```python
def add_check_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de la casilla de verificación desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int |Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal del cuadro de texto desde su columna izquierda, en unidades de píxel.|
| height | int | Altura del cuadro de texto, en unidades de píxel.|
| width | int | Ancho del cuadro de texto, en unidades de píxel.|

###  Ejemplo

```python

# add a CheckBox
checkBox = shapes.add_check_box(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
