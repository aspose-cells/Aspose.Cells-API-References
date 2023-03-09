---
title: auto_fit_row метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 60
url: /ru/python-net/aspose.cells/worksheet/auto_fit_row/
is_root: false
---
##  auto_fit_row(row_index) {#int}
Автоподбор высоты строки.



```python
def auto_fit_row(self, row_index):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| row_index | int | Индекс строки.|
###  Примечания

AutoFitRow — неточная функция.

##  auto_fit_row(row_index, first_column, last_column) {#int-int-int}

Автоподбор высоты строки.



```python
def auto_fit_row(self, row_index, first_column, last_column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| row_index | int | Индекс строки.|
| first_column | int | Индекс первого столбца.|
| last_column | int | Индекс последнего столбца.|
###  Примечания

Этот метод автоматически подбирает строку на основе содержимого диапазона ячеек в строке.

##  auto_fit_row(row_index, first_column, last_column, options) {#int-int-int-AutoFitterOptions}

Автоподбор высоты строки.



```python
def auto_fit_row(self, row_index, first_column, last_column, options):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| row_index | int | Индекс строки.|
| first_column | int | Индекс первого столбца.|
| last_column | int | Индекс последнего столбца.|
| options | [AutoFitterOptions](/cells/ru/python-net/aspose.cells/autofitteroptions) | Параметры автоустановщика|
###  Примечания

Этот метод автоматически подбирает строку на основе содержимого диапазона ячеек в строке.

##  auto_fit_row(start_row, end_row, start_column, end_column) {#int-int-int-int}

Автоподбор высоты строки в прямоугольном диапазоне.



```python
def auto_fit_row(self, start_row, end_row, start_column, end_column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| start_row | int | Индекс начальной строки.|
| end_row | int | Индекс конечной строки.|
| start_column | int | Начальный индекс столбца.|
| end_column | int | Конечный индекс столбца.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Worksheet](/cells/ru/python-net/aspose.cells/worksheet)
