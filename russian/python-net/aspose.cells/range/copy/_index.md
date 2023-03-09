---
title: copy метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/range/copy/
is_root: false
---
##  copy(range) {#Range}
Копирует данные (включая формулы), форматирование, объекты рисования и т. д. из исходного диапазона.



```python
def copy(self, range):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| range | [Range](/cells/ru/python-net/aspose.cells/range) | Источник [Range](/cells/ru/python-net/aspose.cells/range) объект.|

###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A6:A10")
# Copy the range.
range1.copy(range2)
# Save the Excel file
workbook.save("book1.xlsm")

```


##  copy(range, options) {#Range-PasteOptions}
Копирование диапазона со специальными параметрами вставки.



```python
def copy(self, range, options):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| range | [Range](/cells/ru/python-net/aspose.cells/range) | Исходный диапазон.|
| options | [PasteOptions](/cells/ru/python-net/aspose.cells/pasteoptions) | Вставить специальные параметры.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Range](/cells/ru/python-net/aspose.cells/range)
