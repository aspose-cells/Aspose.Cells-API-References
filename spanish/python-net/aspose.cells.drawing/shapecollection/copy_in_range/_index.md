---
title: copy_in_range método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 380
url: /es/python-net/aspose.cells.drawing/shapecollection/copy_in_range/
is_root: false
---
##  copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained) {#ShapeCollection-CellArea-int-int-bool}
Copie formas en el rango al rango de destino.



```python
def copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| source_shapes | [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection) | Formas de origen.|
| ca | [CellArea](/cells/es/python-net/aspose.cells/cellarea) | El rango de la fuente.|
| dest_row | int | El índice de la fila de destino del rango de destino.|
| dest_column | int | La columna dest del rango dest.|
| is_contained | bool | Si solo copia las formas que están contenidas en el rango.<br/> Si es verdadero, solo copia las formas en el rango.<br/> De lo contrario, funciona como MS Office.|

###  Ejemplos

```python
from aspose.cells import CellArea

# add a shape
shapes.add_rectangle(2, 0, 2, 0, 130, 130)
area2 = CellArea()
area2.start_column = 1
area2.start_row = 1
area2.end_column = 5
area2.end_row = 11
# copy
shapes.copy_in_range(shapes, area2, 12, 1, False)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
