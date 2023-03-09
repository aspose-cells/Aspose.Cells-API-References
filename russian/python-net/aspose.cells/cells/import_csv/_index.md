---
title: import_csv метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 630
url: /ru/python-net/aspose.cells/cells/import_csv/
is_root: false
---
##  import_csv(file_name, options, first_row, first_column) {#str-TxtLoadOptions-int-int}
Импортируйте файл CSV в ячейки.



```python
def import_csv(self, file_name, options, first_row, first_column):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| file_name | str | Имя файла CSV.|
| options | [TxtLoadOptions](/cells/ru/python-net/aspose.cells/txtloadoptions) | Параметры загрузки для чтения текстовых файлов|
| first_row | int | Номер строки первой ячейки для импорта.|
| first_column | int | Номер столбца первой ячейки для импорта.|


##  import_csv(stream, options, first_row, first_column) {#io.RawIOBase-TxtLoadOptions-int-int}
Импортируйте файл CSV в ячейки.



```python
def import_csv(self, stream, options, first_row, first_column):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| stream | io.RawIOBase | Файловый поток CSV.|
| options | [TxtLoadOptions](/cells/ru/python-net/aspose.cells/txtloadoptions) | Параметры загрузки для чтения текстовых файлов|
| first_row | int | Номер строки первой ячейки для импорта.|
| first_column | int | Номер столбца первой ячейки для импорта.|


##  import_csv(file_name, splitter, convert_numeric_data, first_row, first_column) {#str-str-bool-int-int}
Импортируйте файл CSV в ячейки.



```python
def import_csv(self, file_name, splitter, convert_numeric_data, first_row, first_column):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| file_name | str | Имя файла CSV.|
| splitter | str | Сплиттер|
| convert_numeric_data | bool |Преобразуется ли строка в текстовом файле в числовые данные.|
| first_row | int | Номер строки первой ячейки для импорта.|
| first_column | int | Номер столбца первой ячейки для импорта.|


##  import_csv(stream, splitter, convert_numeric_data, first_row, first_column) {#io.RawIOBase-str-bool-int-int}
Импортируйте файл CSV в ячейки.



```python
def import_csv(self, stream, splitter, convert_numeric_data, first_row, first_column):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| stream | io.RawIOBase | Файловый поток CSV.|
| splitter | str | Сплиттер|
| convert_numeric_data | bool |Преобразуется ли строка в текстовом файле в числовые данные.|
| first_row | int | Номер строки первой ячейки для импорта.|
| first_column | int | Номер столбца первой ячейки для импорта.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)
