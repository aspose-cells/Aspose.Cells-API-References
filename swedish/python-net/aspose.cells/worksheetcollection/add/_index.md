---
title: add metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/worksheetcollection/add/
is_root: false
---
##  add() {#}
Lägger till ett kalkylblad i samlingen.


###  Returnerar

[Worksheet](/cells/sv/python-net/aspose.cells/worksheet) objektindex.


```python
def add(self):
    ...
```




##  add(type) {#SheetType}
Lägger till ett kalkylblad i samlingen.


###  Returnerar

[Worksheet](/cells/sv/python-net/aspose.cells/worksheet) objektindex.


```python
def add(self, type):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| type | [SheetType](/cells/sv/python-net/aspose.cells/sheettype) | Typ av arbetsblad.|

###  Exempel

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
Lägger till ett kalkylblad i samlingen.


###  Returnerar

[Worksheet](/cells/sv/python-net/aspose.cells/worksheet) objekt.


```python
def add(self, sheet_name):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| sheet_name | str | Arbetsbladsnamn|



###  Se även
* modul [aspose.cells](../../)
* klass [Worksheet](/cells/sv/python-net/aspose.cells/worksheet)
* klass [WorksheetCollection](/cells/sv/python-net/aspose.cells/worksheetcollection)
