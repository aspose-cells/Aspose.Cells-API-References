---
title: طريقة add
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/worksheetcollection/add/
is_root: false
---
##  add() {#}
يضيف ورقة عمل إلى المجموعة.


###  عائدات

[Worksheet](/cells/ar/python-net/aspose.cells/worksheet) فهرس العنصر.


```python
def add(self):
    ...
```




##  add(type) {#SheetType}
يضيف ورقة عمل إلى المجموعة.


###  عائدات

[Worksheet](/cells/ar/python-net/aspose.cells/worksheet) فهرس العنصر.


```python
def add(self, type):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| type | [SheetType](/cells/ar/python-net/aspose.cells/sheettype) | نوع ورقة العمل.|

###  أمثلة

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
يضيف ورقة عمل إلى المجموعة.


###  عائدات

[Worksheet](/cells/ar/python-net/aspose.cells/worksheet) كائن.


```python
def add(self, sheet_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| sheet_name | str | اسم ورقة العمل|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Worksheet](/cells/ar/python-net/aspose.cells/worksheet)
* فئة [WorksheetCollection](/cells/ar/python-net/aspose.cells/worksheetcollection)
