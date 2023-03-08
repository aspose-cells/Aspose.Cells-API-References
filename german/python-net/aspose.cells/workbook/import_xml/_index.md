---
title: import_xml Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 220
url: /de/python-net/aspose.cells/workbook/import_xml/
is_root: false
---
##  import_xml(url, sheet_name, row, col) {#str-str-int-int}
Importiert/aktualisiert eine XML-Datendatei in die Arbeitsmappe.



```python
def import_xml(self, url, sheet_name, row, col):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| url | str | URL/Pfad der XML-Datei.|
| sheet_name | str | der Name des Zielblatts.|
| row | int | die Zielzeile|
| col | int | die Zielspalte|

###  Beispiel

Der folgende Code importiert XML-Daten in das Arbeitsblatt „Blatt 1“ um Cell A1.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
wb.import_xml("xml.xml", "Sheet1", 0, 0)
wb.save("output.xlsx")

```


##  import_xml(stream, sheet_name, row, col) {#io.RawIOBase-str-int-int}
Importiert/aktualisiert eine XML-Datendatei in die Arbeitsmappe.



```python
def import_xml(self, stream, sheet_name, row, col):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| stream | io.RawIOBase | den XML-Dateistream.|
| sheet_name | str | der Name des Zielblatts.|
| row | int | die Zielzeile.|
| col | int |die Zielspalte.|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Workbook](/cells/de/python-net/aspose.cells/workbook)
