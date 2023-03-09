---
title: import_xml metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 220
url: /sv/python-net/aspose.cells/workbook/import_xml/
is_root: false
---
##  import_xml(url, sheet_name, row, col) {#str-str-int-int}
Importerar/uppdaterar en XML-datafil till arbetsboken.



```python
def import_xml(self, url, sheet_name, row, col):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| url | str | URL/sökväg till xml-filen.|
| sheet_name | str | destinationsbladets namn.|
| row | int | destinationsraden|
| col | int | destinationskolumnen|

###  Exempel

Följande kod importerar xml-data till kalkylblad 'Sheet 1' på Cell A1.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
wb.import_xml("xml.xml", "Sheet1", 0, 0)
wb.save("output.xlsx")

```


##  import_xml(stream, sheet_name, row, col) {#io.RawIOBase-str-int-int}
Importerar/uppdaterar en XML-datafil till arbetsboken.



```python
def import_xml(self, stream, sheet_name, row, col):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase | xml-filströmmen.|
| sheet_name | str | destinationsbladets namn.|
| row | int | destinationsraden.|
| col | int | destinationskolumnen.|



###  Se även
* modul [aspose.cells](../../)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
