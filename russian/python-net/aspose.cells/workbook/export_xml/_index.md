---
title: export_xml метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 140
url: /ru/python-net/aspose.cells/workbook/export_xml/
is_root: false
---
##  export_xml(map_name, path) {#str-str}
Экспорт данных XML, связанных указанной картой XML.



```python
def export_xml(self, map_name, path):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| map_name | str | имя карты XML, которую необходимо экспортировать|
| path | str | путь экспорта|

###  Пример

Следующий код экспортирует данные, связанные с первым XmlMap.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
# Make sure that the source xlsx file contains a XmlMap.
xmlMap = wb.worksheets.xml_maps[0]
wb.export_xml(xmlMap.name, "output.xml")

```


##  export_xml(map_name, stream) {#str-io.RawIOBase}
Экспорт XML-данных.



```python
def export_xml(self, map_name, stream):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| map_name | str | имя карты XML, которую необходимо экспортировать|
| stream | io.RawIOBase | экспортный поток|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
