---
title: delete_in_range метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 400
url: /ru/python-net/aspose.cells.drawing/shapecollection/delete_in_range/
is_root: false
---
##  delete_in_range(ca) {#CellArea}
Удалить фигуры в диапазоне. Фигуры комментариев не будут удалены.



```python
def delete_in_range(self, ca):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| ca | [CellArea](/cells/ru/python-net/aspose.cells/cellarea) |Диапазон. Если фигуры содержатся в диапазоне, они будут удалены.|

###  Пример

```python
from aspose.cells import CellArea

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
area3 = CellArea()
area3.start_column = 0
area3.start_row = 5
area3.end_column = 5
area3.end_row = 8
# del
shapes.delete_in_range(area3)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)
