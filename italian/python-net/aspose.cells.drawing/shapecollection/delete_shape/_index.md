---
title: metodo delete_shape
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 410
url: /it/python-net/aspose.cells.drawing/shapecollection/delete_shape/
is_root: false
---
##  delete_shape(shape) {#Shape}
Elimina una forma. Se la forma è nel gruppo o è una forma di commento, non verrà eliminata.



```python
def delete_shape(self, shape):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| shape | [Shape](/cells/it/python-net/aspose.cells.drawing/shape) |  |

###  Esempio

```python

# add first shape
firstShape = shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
secondShape = shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# del
shapes.delete_shape(firstShape)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)
