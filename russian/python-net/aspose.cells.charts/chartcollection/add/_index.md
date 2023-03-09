---
title: add метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.charts/chartcollection/add/
is_root: false
---
##  add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column) {#ChartType-int-int-int-int}
Добавляет диаграмму в коллекцию.


###  Возвращает

[Chart](/cells/ru/python-net/aspose.cells.charts/chart) индекс объекта.


```python
def add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [ChartType](/cells/ru/python-net/aspose.cells.charts/charttype) | Тип диаграммы|
| upper_left_row | int | Индекс верхней левой строки.|
| upper_left_column | int |Индекс левого верхнего столбца.|
| lower_right_row | int | Нижний индекс правой строки|
| lower_right_column | int | Индекс нижнего правого столбца|


##  add(type, data_range, top_row, left_column, right_row, bottom_column) {#ChartType-str-int-int-int-int}
Добавляет диаграмму в коллекцию.


###  Возвращает

[Chart](/cells/ru/python-net/aspose.cells.charts/chart) индекс объекта.


```python
def add(self, type, data_range, top_row, left_column, right_row, bottom_column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [ChartType](/cells/ru/python-net/aspose.cells.charts/charttype) | Тип диаграммы|
| data_range | str |Указывает диапазон данных диаграммы|
| top_row | int | Индекс верхней левой строки.|
| left_column | int |Индекс левого верхнего столбца.|
| right_row | int | Нижний индекс правой строки|
| bottom_column | int | Индекс нижнего правого столбца|
###  Примечания

ПРИМЕЧАНИЕ. Этот элемент устарел. Вместо,
пожалуйста, используйте свойство [ChartCollection.add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/ru/python-net/aspose.cells.charts/chartcollection/add).
Это свойство будет удалено через 12 месяцев, начиная с мая 2022 года.
Aspose приносит извинения за возможные неудобства.

##  add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#bytes-str-bool-int-int-int-int}
Добавляет диаграмму с предустановленным шаблоном.


###  Возвращает

[Chart](/cells/ru/python-net/aspose.cells.charts/chart) индекс объекта.


```python
def add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| data | bytes | Данные файла шаблона диаграммы (.crtx).|
| data_range | str |Указывает диапазон данных диаграммы|
| is_vertical | bool | Указывает, следует ли отображать серию из диапазона значений ячеек по строке или по столбцу.|
| top_row | int | Индекс верхней левой строки.|
| left_column | int |Индекс левого верхнего столбца.|
| right_row | int | Нижний индекс правой строки|
| bottom_column | int | Индекс нижнего правого столбца|


##  add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#ChartType-str-bool-int-int-int-int}
Добавляет диаграмму в коллекцию.


###  Возвращает

[Chart](/cells/ru/python-net/aspose.cells.charts/chart) индекс объекта.


```python
def add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [ChartType](/cells/ru/python-net/aspose.cells.charts/charttype) | Тип диаграммы|
| data_range | str |Указывает диапазон данных диаграммы|
| is_vertical | bool | Указывает, следует ли отображать серию из диапазона значений ячеек по строке или по столбцу.|
| top_row | int | Индекс верхней левой строки.|
| left_column | int |Индекс левого верхнего столбца.|
| right_row | int | Нижний индекс правой строки|
| bottom_column | int | Индекс нижнего правого столбца|



###  Смотрите также
* модуль [aspose.cells.charts](../../)
* класс [Chart](/cells/ru/python-net/aspose.cells.charts/chart)
* класс [ChartCollection](/cells/ru/python-net/aspose.cells.charts/chartcollection)
