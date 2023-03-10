---
title: add_copy método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 90
url: /es/python-net/aspose.cells.drawing/shapecollection/add_copy/
is_root: false
---
##  add_copy(source_shape, upper_left_row, top, upper_left_column, left) {#Shape-int-int-int-int}
Agrega y copia una forma a la hoja de trabajo.


###  Devoluciones

El nuevo índice de objeto de forma.


```python
def add_copy(self, source_shape, upper_left_row, top, upper_left_column, left):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| source_shape | [Shape](/cells/es/python-net/aspose.cells.drawing/shape) | Forma de fuente.|
| upper_left_row | int | Índice de la fila superior izquierda.|
| top | int |Representa el desplazamiento vertical de la casilla de verificación desde su fila izquierda, en unidades de píxel.|
| upper_left_column | int | Índice de la columna superior izquierda.|
| left | int | Representa el desplazamiento horizontal del cuadro de texto desde su columna izquierda, en unidades de píxel.|

###  Ejemplo

```python

# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)
# copy
shapes.add_copy(rectangle, 7, 0, 7, 0)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
