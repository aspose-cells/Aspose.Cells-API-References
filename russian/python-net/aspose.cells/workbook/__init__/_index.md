---
title: Workbook конструктор
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 10
url: /ru/python-net/aspose.cells/workbook/__init__/
is_root: false
---
##  Workbook() {#}
Инициализирует новый экземпляр класса [Workbook](/cells/ru/python-net/aspose.cells/workbook).



```python
def __init__(self):
    ...
```


###  Примечания

Тип формата файла по умолчанию — Xlsx. Чтобы создать файл другого формата, используйте Workbook (FileFormatType).
###  Примеры


В следующем коде показано, как использовать конструктор Workbook для создания и инициализации нового экземпляра класса.

```python
from aspose.cells import Workbook

workbook = Workbook()

```


##  Workbook(file_format_type) {#FileFormatType}
Инициализирует новый экземпляр класса [Workbook](/cells/ru/python-net/aspose.cells/workbook).



```python
def __init__(self, file_format_type):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| file_format_type | [FileFormatType](/cells/ru/python-net/aspose.cells/fileformattype) | Новый формат файла.|
###  Примечания

Тип формата файла по умолчанию — Excel97To2003.
###  Примеры


В следующем коде показано, как использовать конструктор Workbook для создания и инициализации нового экземпляра класса.

```python
from aspose.cells import FileFormatType, Workbook

workbook = Workbook(FileFormatType.XLSX)

```


##  Workbook(file) {#str}
Инициализирует новый экземпляр класса [Workbook](/cells/ru/python-net/aspose.cells/workbook) и открывает файл.



```python
def __init__(self, file):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| file | str | Имя файла.|


##  Workbook(stream) {#io.RawIOBase}
Инициализирует новый экземпляр класса [Workbook](/cells/ru/python-net/aspose.cells/workbook) и открывает поток.



```python
def __init__(self, stream):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| stream | io.RawIOBase | Поток.|


##  Workbook(file, load_options) {#str-LoadOptions}
Инициализирует новый экземпляр класса [Workbook](/cells/ru/python-net/aspose.cells/workbook) и открывает файл.



```python
def __init__(self, file, load_options):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| file | str | Имя файла.|
| load_options | [LoadOptions](/cells/ru/python-net/aspose.cells/loadoptions) | Параметры загрузки|


##  Workbook(stream, load_options) {#io.RawIOBase-LoadOptions}
Инициализирует новый экземпляр класса [Workbook](/cells/ru/python-net/aspose.cells/workbook) и открытый поток.



```python
def __init__(self, stream, load_options):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| stream | io.RawIOBase | Поток.|
| load_options | [LoadOptions](/cells/ru/python-net/aspose.cells/loadoptions) | Параметры загрузки|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
