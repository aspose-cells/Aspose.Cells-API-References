---
title: sort метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/datasorter/sort/
is_root: false
---
##  sort() {#}
Отсортируйте данные в диапазоне.


###  Возвращает

исходные индексы (абсолютная позиция, например, столбец A равен 0, B равен 1,...) отсортированных строк/столбцов.
Если этой операцией сортировки не нужно перемещать строки/столбцы, будет возвращено значение null.


```python
def sort(self):
    ...
```




##  sort(cells, area) {#Cells-CellArea}
Сортировка данных области.


###  Возвращает

исходные индексы (абсолютная позиция, например, столбец A равен 0, B равен 1,...) отсортированных строк/столбцов.
Если этой операцией сортировки не нужно перемещать строки/столбцы, будет возвращено значение null.


```python
def sort(self, cells, area):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| cells | [Cells](/cells/ru/python-net/aspose.cells/cells) | Ячейки содержат область данных.|
| area | [CellArea](/cells/ru/python-net/aspose.cells/cellarea) | Площадь, необходимая для сортировки|


##  sort(cells, start_row, start_column, end_row, end_column) {#Cells-int-int-int-int}
Сортирует данные области.


###  Возвращает

исходные индексы (абсолютная позиция, например, столбец A равен 0, B равен 1,...) отсортированных строк/столбцов.
Если этой операцией сортировки не нужно перемещать строки/столбцы, будет возвращено значение null.


```python
def sort(self, cells, start_row, start_column, end_row, end_column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| cells | [Cells](/cells/ru/python-net/aspose.cells/cells) | Ячейки содержат область данных.|
| start_row | int | Стартовый ряд площади.|
| start_column | int | Начальный столбец области.|
| end_row | int | Крайний ряд площади.|
| end_column | int | Конечная колонка области.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [DataSorter](/cells/ru/python-net/aspose.cells/datasorter)
