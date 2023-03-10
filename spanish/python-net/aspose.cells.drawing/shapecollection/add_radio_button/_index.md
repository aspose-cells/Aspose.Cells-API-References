---
title: add_radio_button método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 230
url: /es/python-net/aspose.cells.drawing/shapecollection/add_radio_button/
is_root: false
---
##  add_radio_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega un RadioButton a la hoja de trabajo.


###  Devoluciones

Un objeto Botón de radio.


```python
def add_radio_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical de RadioButton desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal de RadioButton desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura de RadioButton, en unidades de píxel.|
| width | int | Representa el ancho de RadioButton, en unidades de píxel.|

###  Ejemplo

```python

# add a radio button
radioButton = shapes.add_radio_button(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
