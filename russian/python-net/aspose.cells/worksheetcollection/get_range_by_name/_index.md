---
title: get_range_by_name метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 120
url: /ru/python-net/aspose.cells/worksheetcollection/get_range_by_name/
is_root: false
---
##  get_range_by_name(range_name) {#str}
Получает объект Range по заданному имени.


###  Возвращает

Объект диапазона.


Возвращает null, если именованный диапазон не существует.


```python
def get_range_by_name(self, range_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| range_name | str | Название диапазона.|


##  get_range_by_name(range_name, current_sheet_index, include_table) {#str-int-bool}
Получает [Range](/cells/ru/python-net/aspose.cells/range) по заданному имени или имени таблицы


###  Возвращает




```python
def get_range_by_name(self, range_name, current_sheet_index, include_table):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| range_name | str | Имя диапазона или имя таблицы.|
| current_sheet_index | int | Индекс листа. -1 представляет глобальный .|
| include_table | bool | Указывает, проверяются ли все таблицы.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Range](/cells/ru/python-net/aspose.cells/range)
* класс [WorksheetCollection](/cells/ru/python-net/aspose.cells/worksheetcollection)
