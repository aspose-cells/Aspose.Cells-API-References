---
title: add_text_box método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 310
url: /es/python-net/aspose.cells.drawing/shapecollection/add_text_box/
is_root: false
---
##  add_text_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Agrega un cuadro de texto a la hoja de cálculo.


###  Devoluciones

Un objeto [TextBox](/cells/es/python-net/aspose.cells.drawing/textbox).


```python
def add_text_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int | Representa el desplazamiento vertical del cuadro de texto desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal del cuadro de texto desde su columna izquierda, en unidades de píxel.|
| height | int | Representa la altura del cuadro de texto, en unidades de píxel.|
| width | int | Representa el ancho del cuadro de texto, en unidades de píxel.|

###  Ejemplos

```python

# add a TextBox
textBox = shapes.add_text_box(1, 0, 1, 0, 100, 50)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
* clase [TextBox](/cells/es/python-net/aspose.cells.drawing/textbox)
