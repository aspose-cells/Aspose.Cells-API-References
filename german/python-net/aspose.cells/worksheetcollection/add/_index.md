---
title: add Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells/worksheetcollection/add/
is_root: false
---
##  add() {#}
Fügt der Sammlung ein Arbeitsblatt hinzu.


###  Kehrt zurück

[Worksheet](/cells/de/python-net/aspose.cells/worksheet) Objektindex.


```python
def add(self):
    ...
```




##  add(type) {#SheetType}
Fügt der Sammlung ein Arbeitsblatt hinzu.


###  Kehrt zurück

[Worksheet](/cells/de/python-net/aspose.cells/worksheet) Objektindex.


```python
def add(self, type):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [SheetType](/cells/de/python-net/aspose.cells/sheettype) | Arbeitsblatttyp.|

###  Beispiel

```python
from aspose.cells import SheetType, Workbook
from aspose.cells.charts import ChartType

workbook = Workbook()
workbook.worksheets.add(SheetType.CHART)
cells = workbook.worksheets[0].cells
cells.get("c2").put_value(5000)
cells.get("c3").put_value(3000)
cells.get("c4").put_value(4000)
cells.get("c5").put_value(5000)
cells.get("c6").put_value(6000)
charts = workbook.worksheets[1].charts
chartIndex = charts.add(ChartType.COLUMN, 10, 10, 20, 20)
chart = charts[chartIndex]
chart.n_series.add("Sheet1!C2:C6", True)

```


##  add(sheet_name) {#str}
Fügt der Sammlung ein Arbeitsblatt hinzu.


###  Kehrt zurück

[Worksheet](/cells/de/python-net/aspose.cells/worksheet) Objekt.


```python
def add(self, sheet_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| sheet_name | str | Arbeitsblattname|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Worksheet](/cells/de/python-net/aspose.cells/worksheet)
* Klasse [WorksheetCollection](/cells/de/python-net/aspose.cells/worksheetcollection)
