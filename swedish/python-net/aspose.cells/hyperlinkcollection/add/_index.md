---
title: add metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/hyperlinkcollection/add/
is_root: false
---
##  add(cell_name, total_rows, total_columns, address) {#str-int-int-str}
Lägger till en hyperlänk till en angiven cell eller ett cellintervall.


###  Returnerar

[Hyperlink](/cells/sv/python-net/aspose.cells/hyperlink) objektindex.


```python
def add(self, cell_name, total_rows, total_columns, address):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| cell_name | str | Cell namn.|
| total_rows | int | Antal rader i detta hyperlänksintervall.|
| total_columns | int | Antal kolumner i detta hyperlänksintervall.|
| address | str | Adress till hyperlänken.|


##  add(first_row, first_column, total_rows, total_columns, address) {#int-int-int-int-str}
Lägger till en hyperlänk till en angiven cell eller ett cellintervall.


###  Returnerar

[Hyperlink](/cells/sv/python-net/aspose.cells/hyperlink) objektindex.


```python
def add(self, first_row, first_column, total_rows, total_columns, address):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| first_row | int | Första raden i hyperlänksintervallet.|
| first_column | int | Första kolumnen i hyperlänksintervallet.|
| total_rows | int | Antal rader i detta hyperlänksintervall.|
| total_columns | int | Antal kolumner i detta hyperlänksintervall.|
| address | str | Adress till hyperlänken.|

###  Exempel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
excel = Workbook()
worksheet = excel.worksheets[0]
worksheet.hyperlinks.add("A4", 1, 1, "http://www.aspose.com")
worksheet.hyperlinks.add("A5", 1, 1, "c:\\book1.xls")

```


##  add(start_cell_name, end_cell_name, address, text_to_display, screen_tip) {#str-str-str-str-str}
Lägger till en hyperlänk till en angiven cell eller ett cellintervall.


###  Returnerar

[Hyperlink](/cells/sv/python-net/aspose.cells/hyperlink) objektindex.


```python
def add(self, start_cell_name, end_cell_name, address, text_to_display, screen_tip):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| start_cell_name | str | Den övre vänstra cellen i intervallet.|
| end_cell_name | str | Den nedre högra cellen i intervallet.|
| address | str | Adress till hyperlänken.|
| text_to_display | str | Texten som ska visas för den angivna hyperlänken.|
| screen_tip | str |Skärmtipstexten för den angivna hyperlänken.|



###  Se även
* modul [aspose.cells](../../)
* klass [Hyperlink](/cells/sv/python-net/aspose.cells/hyperlink)
* klass [HyperlinkCollection](/cells/sv/python-net/aspose.cells/hyperlinkcollection)
