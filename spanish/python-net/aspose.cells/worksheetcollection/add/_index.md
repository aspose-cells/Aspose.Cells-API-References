---
title: add método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/worksheetcollection/add/
is_root: false
---
##  add() {#}
Agrega una hoja de cálculo a la colección.


###  Devoluciones

[Worksheet](/cells/es/python-net/aspose.cells/worksheet) índice de objetos.


```python
def add(self):
    ...
```




##  add(type) {#SheetType}
Agrega una hoja de cálculo a la colección.


###  Devoluciones

[Worksheet](/cells/es/python-net/aspose.cells/worksheet) índice de objetos.


```python
def add(self, type):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| type | [SheetType](/cells/es/python-net/aspose.cells/sheettype) | Tipo de hoja de trabajo.|

###  Ejemplo

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
Agrega una hoja de cálculo a la colección.


###  Devoluciones

[Worksheet](/cells/es/python-net/aspose.cells/worksheet) objeto.


```python
def add(self, sheet_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| sheet_name | str | Nombre de la hoja de trabajo|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Worksheet](/cells/es/python-net/aspose.cells/worksheet)
* clase [WorksheetCollection](/cells/es/python-net/aspose.cells/worksheetcollection)
