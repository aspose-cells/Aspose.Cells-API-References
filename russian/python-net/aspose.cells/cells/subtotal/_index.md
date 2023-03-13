---
title: subtotal метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 920
url: /ru/python-net/aspose.cells/cells/subtotal/
is_root: false
---
##  subtotal(ca, group_by, function, total_list) {#CellArea-int-ConsolidationFunction-list}
Создает промежуточные итоги для диапазона.



```python
def subtotal(self, ca, group_by, function, total_list):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| ca | [CellArea](/cells/ru/python-net/aspose.cells/cellarea) | Диапазон|
| group_by | int | Поле для группировки в виде целочисленного смещения, отсчитываемого от нуля.|
| function | [ConsolidationFunction](/cells/ru/python-net/aspose.cells/consolidationfunction) | Функция промежуточного итога.|
| total_list | list | Массив отсчитываемых от нуля смещений полей, указывающий поля, к которым добавляются промежуточные итоги.|


##  subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data) {#CellArea-int-ConsolidationFunction-list-bool-bool-bool}
Создает промежуточные итоги для диапазона.



```python
def subtotal(self, ca, group_by, function, total_list, replace, page_breaks, summary_below_data):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| ca | [CellArea](/cells/ru/python-net/aspose.cells/cellarea) | Диапазон|
| group_by | int | Поле для группировки в виде целочисленного смещения, отсчитываемого от нуля.|
| function | [ConsolidationFunction](/cells/ru/python-net/aspose.cells/consolidationfunction) | Функция промежуточного итога.|
| total_list | list | Массив отсчитываемых от нуля смещений полей, указывающий поля, к которым добавляются промежуточные итоги.|
| replace | bool | Указывает, заменять ли текущие промежуточные итоги|
| page_breaks | bool | Указывает, добавлять ли разрыв страницы между группами|
| summary_below_data | bool | Указывает, следует ли добавлять сводку ниже данных.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)
