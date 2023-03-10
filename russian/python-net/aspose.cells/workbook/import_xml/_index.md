---
title: import_xml метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 220
url: /ru/python-net/aspose.cells/workbook/import_xml/
is_root: false
---
##  import_xml(url, sheet_name, row, col) {#str-str-int-int}
Импортирует/обновляет файл данных XML в книгу.



```python
def import_xml(self, url, sheet_name, row, col):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| url | str | URL-адрес/путь XML-файла.|
| sheet_name | str | имя целевого листа.|
| row | int | строка назначения|
| col | int | столбец назначения|

###  Пример

Следующий код импортирует данные XML в рабочий лист «Лист 1» по адресу Cell A1.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
wb.import_xml("xml.xml", "Sheet1", 0, 0)
wb.save("output.xlsx")

```


##  import_xml(stream, sheet_name, row, col) {#io.RawIOBase-str-int-int}
Импортирует/обновляет файл данных XML в книгу.



```python
def import_xml(self, stream, sheet_name, row, col):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| stream | io.RawIOBase | поток xml-файлов.|
| sheet_name | str | имя целевого листа.|
| row | int | строка назначения.|
| col | int | столбец назначения.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
