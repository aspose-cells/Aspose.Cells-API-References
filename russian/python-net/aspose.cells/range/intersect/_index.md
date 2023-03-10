---
title: intersect метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 110
url: /ru/python-net/aspose.cells/range/intersect/
is_root: false
---
##  intersect(range) {#Range}
Возвращает объект [Range](/cells/ru/python-net/aspose.cells/range), представляющий прямоугольное пересечение двух диапазонов.


###  Возвращает

Возвращает объект [Range](/cells/ru/python-net/aspose.cells/range)


```python
def intersect(self, range):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| range | [Range](/cells/ru/python-net/aspose.cells/range) | Пересекающийся диапазон.|
###  Примечания

Если два диапазона не пересекаются, возвращает null.
###  Пример


```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A3:A10")
# Get intersected range of the two ranges.
intersectRange = range1.intersect(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Range](/cells/ru/python-net/aspose.cells/range)
