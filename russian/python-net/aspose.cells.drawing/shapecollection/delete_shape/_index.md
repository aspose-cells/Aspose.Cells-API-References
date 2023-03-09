---
title: delete_shape метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 410
url: /ru/python-net/aspose.cells.drawing/shapecollection/delete_shape/
is_root: false
---
##  delete_shape(shape) {#Shape}
Удалить фигуру. Если фигура находится в группе или является фигурой комментария, она не будет удалена.



```python
def delete_shape(self, shape):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| shape | [Shape](/cells/ru/python-net/aspose.cells.drawing/shape) |  |

###  Пример

```python

# add first shape
firstShape = shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
secondShape = shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# del
shapes.delete_shape(firstShape)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)
