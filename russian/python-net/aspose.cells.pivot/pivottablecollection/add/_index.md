---
title: add метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.pivot/pivottablecollection/add/
is_root: false
---
##  add(source_data, dest_cell_name, table_name) {#str-str-str}
Добавляет новый кэш сводной таблицы в коллекцию сводных кешей.


###  Возвращает

Новый добавленный кеш-индекс.


```python
def add(self, source_data, dest_cell_name, table_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| source_data | str | Данные для нового кэша сводной таблицы.|
| dest_cell_name | str |Ячейка в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| table_name | str | Имя нового отчета сводной таблицы.|


##  add(pivot_table, dest_cell_name, table_name) {#PivotTable-str-str}
Добавляет новый объект сводной таблицы в коллекцию из другой сводной таблицы.


###  Возвращает

Новый добавленный индекс сводной таблицы.


```python
def add(self, pivot_table, dest_cell_name, table_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/ru/python-net/aspose.cells.pivot/pivottable) | Исходная сводная таблица.|
| dest_cell_name | str |Ячейка в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| table_name | str | Имя нового отчета сводной таблицы.|


##  add(source_data, dest_cell_name, table_name, use_same_source) {#str-str-str-bool}
Добавляет новый кэш сводной таблицы в коллекцию сводных кешей.


###  Возвращает

Новый добавленный кеш-индекс.


```python
def add(self, source_data, dest_cell_name, table_name, use_same_source):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| source_data | str | Данные для нового кэша сводной таблицы.|
| dest_cell_name | str |Ячейка в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| table_name | str | Имя нового отчета сводной таблицы.|
| use_same_source | bool | Указывает, используется ли тот же источник данных, когда другая существующая сводная таблица использовала этот источник данных.<br/> Если свойство истинно, оно сэкономит память.|


##  add(source_data, row, column, table_name) {#str-int-int-str}
Добавляет новый кэш сводной таблицы в коллекцию сводных кешей.


###  Возвращает

Новый добавленный кеш-индекс.


```python
def add(self, source_data, row, column, table_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| source_data | str | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8.|
| row | int | Индекс строки ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| column | int | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| table_name | str | Имя нового отчета сводной таблицы.|


##  add(pivot_table, row, column, table_name) {#PivotTable-int-int-str}
Добавляет новый объект сводной таблицы в коллекцию из другой сводной таблицы.


###  Возвращает

Новый добавленный индекс сводной таблицы.


```python
def add(self, pivot_table, row, column, table_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/ru/python-net/aspose.cells.pivot/pivottable) | Исходная сводная таблица.|
| row | int | Индекс строки ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| column | int | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| table_name | str | Имя нового отчета сводной таблицы.|


##  add(source_data, row, column, table_name, use_same_source) {#str-int-int-str-bool}
Добавляет новый кэш сводной таблицы в коллекцию сводных кешей.


###  Возвращает

Новый добавленный кеш-индекс.


```python
def add(self, source_data, row, column, table_name, use_same_source):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| source_data | str | Диапазон ячеек данных для новой сводной таблицы. Пример: Sheet1!A1:C8.|
| row | int | Индекс строки ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| column | int | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| table_name | str | Имя нового отчета сводной таблицы.|
| use_same_source | bool | Указывает, используется ли тот же источник данных, когда другая существующая сводная таблица использовала этот источник данных.<br/> Если свойство истинно, оно сэкономит память.|


##  add(source_data, is_auto_page, page_fields, dest_cell_name, table_name) {#list-bool-PivotPageFields-str-str}
Добавляет новый объект сводной таблицы в коллекцию с несколькими диапазонами консолидации в качестве источника данных.


###  Возвращает

Новый добавленный индекс сводной таблицы.


```python
def add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| source_data | list | Несколько диапазонов консолидации, например {"Лист1!A1:C8","Лист2!A1:B8"} |
| is_auto_page | bool | Будет ли автоматически создаваться одностраничное поле.<br/>Если true, следующие параметры pageFields будут игнорироваться.|
| page_fields | [PivotPageFields](/cells/ru/python-net/aspose.cells.pivot/pivotpagefields) | Элементы поля сводной страницы.|
| dest_cell_name | str | destCellName Имя нового отчета сводной таблицы.|
| table_name | str | имя нового отчета сводной таблицы.|


##  add(source_data, is_auto_page, page_fields, row, column, table_name) {#list-bool-PivotPageFields-int-int-str}
Добавляет новый объект сводной таблицы в коллекцию с несколькими диапазонами консолидации в качестве источника данных.


###  Возвращает

Новый добавленный индекс сводной таблицы.


```python
def add(self, source_data, is_auto_page, page_fields, row, column, table_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| source_data | list | Несколько диапазонов консолидации, например {"Лист1!A1:C8","Лист2!A1:B8"} |
| is_auto_page | bool | Будет ли автоматически создаваться одностраничное поле.<br/> Если true, следующие параметры pageFields будут игнорироваться.|
| page_fields | [PivotPageFields](/cells/ru/python-net/aspose.cells.pivot/pivotpagefields) | Элементы поля сводной страницы.|
| row | int | Индекс строки ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| column | int | Индекс столбца ячейки в верхнем левом углу диапазона назначения отчета сводной таблицы.|
| table_name | str | Имя нового отчета сводной таблицы.|



###  Смотрите также
* модуль [aspose.cells.pivot](../../)
* класс [PivotTableCollection](/cells/ru/python-net/aspose.cells.pivot/pivottablecollection)
