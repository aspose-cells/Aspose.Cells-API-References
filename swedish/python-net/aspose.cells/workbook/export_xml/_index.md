---
title: export_xml metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 140
url: /sv/python-net/aspose.cells/workbook/export_xml/
is_root: false
---
##  export_xml(map_name, path) {#str-str}
Exportera XML-data länkade av den angivna XML-kartan.



```python
def export_xml(self, map_name, path):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| map_name | str | namnet på XML-kartan som behöver exporteras|
| path | str | exportvägen|

###  Exempel

Följande kod exporterade data som länkades av den första XmlMap.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
# Make sure that the source xlsx file contains a XmlMap.
xmlMap = wb.worksheets.xml_maps[0]
wb.export_xml(xmlMap.name, "output.xml")

```


##  export_xml(map_name, stream) {#str-io.RawIOBase}
Exportera XML-data.



```python
def export_xml(self, map_name, stream):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| map_name | str | namnet på XML-kartan som behöver exporteras|
| stream | io.RawIOBase | exportströmmen|



###  Se även
* modul [aspose.cells](../../)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
