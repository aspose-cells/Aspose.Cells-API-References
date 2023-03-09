---
title: add yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/worksheetcollection/add/
is_root: false
---
##  add() {#}
Koleksiyona bir çalışma sayfası ekler.


###  İadeler

[Worksheet](/cells/tr/python-net/aspose.cells/worksheet) nesne dizini.


```python
def add(self):
    ...
```




##  add(type) {#SheetType}
Koleksiyona bir çalışma sayfası ekler.


###  İadeler

[Worksheet](/cells/tr/python-net/aspose.cells/worksheet) nesne dizini.


```python
def add(self, type):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [SheetType](/cells/tr/python-net/aspose.cells/sheettype) | Çalışma sayfası türü.|

###  Örnek

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
Koleksiyona bir çalışma sayfası ekler.


###  İadeler

[Worksheet](/cells/tr/python-net/aspose.cells/worksheet) nesne.


```python
def add(self, sheet_name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| sheet_name | str | çalışma sayfası adı|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Worksheet](/cells/tr/python-net/aspose.cells/worksheet)
* sınıf [WorksheetCollection](/cells/tr/python-net/aspose.cells/worksheetcollection)
