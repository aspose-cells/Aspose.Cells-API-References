##add method
## add(self) {#}
Adds a worksheet to the collection.
### Returns
[`Worksheet`](/cells/python-net/aspose.cells/worksheet) object index.
```python
def add(self):
...
```
## add(self, type) {#aspose.cells.SheetType}
Adds a worksheet to the collection.
### Returns
[`Worksheet`](/cells/python-net/aspose.cells/worksheet) object index.
```python
def add(self, type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.SheetType | Worksheet type. |
### Example
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
## add(self, sheet_name) {#System.String}
Adds a worksheet to the collection.
### Returns
[`Worksheet`](/cells/python-net/aspose.cells/worksheet) object.
```python
def add(self, sheet_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| sheet_name | System.String | Worksheet name |
### See Also
* module [`aspose.cells`](../../)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)
* class [`WorksheetCollection`](/cells/python-net/aspose.cells/worksheetcollection)
