---
title: copy_in_range метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 380
url: /ru/python-net/aspose.cells.drawing/shapecollection/copy_in_range/
is_root: false
---
##  copy_in_range(source_shapes, ca, dest_row, dest_column, is_contained) {#ShapeCollection-CellArea-int-int-bool}
Скопируйте фигуры из диапазона в целевой диапазон.



```python
def copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| source_shapes | [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection) | Исходные формы.|
| ca | [CellArea](/cells/ru/python-net/aspose.cells/cellarea) | Исходный диапазон.|
| dest_row | int | Индекс строки назначения диапазона назначения.|
| dest_column | int | Столбец назначения диапазона назначения.|
| is_contained | bool | Копировать ли только те фигуры, которые содержатся в диапазоне.<br/> Если true, копируются только фигуры в диапазоне.<br/> В противном случае он работает как MS Office.|

###  Пример

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



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)
