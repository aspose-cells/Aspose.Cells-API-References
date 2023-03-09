---
title: delete_shape método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 410
url: /es/python-net/aspose.cells.drawing/shapecollection/delete_shape/
is_root: false
---
##  delete_shape(shape) {#Shape}
Eliminar una forma Si la forma está en el grupo o es una forma de comentario, no se eliminará.



```python
def delete_shape(self, shape):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| shape | [Shape](/cells/es/python-net/aspose.cells.drawing/shape) |  |

###  Ejemplos

```python

# add first shape
firstShape = shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
secondShape = shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# del
shapes.delete_shape(firstShape)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
