##add method
## add(self, pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-System.String-System.String}
Add a new Timeline using PivotTable as data source
### Returns
The new add Timeline index
```python
def add(self, pivot, dest_cell_name, base_field_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| dest_cell_name | System.String | The cell name in the upper-left corner of the Timeline range. |
| base_field_name | System.String | The name of PivotField in PivotTable.BaseFields |
### Example
```python
# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i15", "date")
```
## add(self, pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-System.String-int}
Add a new Timeline using PivotTable as data source
### Returns
The new add Timeline index
```python
def add(self, pivot, dest_cell_name, base_field_index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| dest_cell_name | System.String | The cell name in the upper-left corner of the Timeline range. |
| base_field_index | int | The index of PivotField in PivotTable.BaseFields |
### Example
```python
# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i5", 1)
```
## add(self, pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-System.String-aspose.cells.pivot.PivotField}
Add a new Timeline using PivotTable as data source
### Returns
The new add Timeline index
```python
def add(self, pivot, dest_cell_name, base_field):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| dest_cell_name | System.String | The cell name in the upper-left corner of the Timeline range. |
| base_field | aspose.cells.pivot.PivotField | The PivotField in PivotTable.BaseFields |
### Example
```python
# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i10", pivot.base_fields[1])
```
## add(self, pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-System.String}
Add a new Timeline using PivotTable as data source
### Returns
The new add Timeline index
```python
def add(self, pivot, row, column, base_field_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Timeline range. |
| column | int | Column index of the cell in the upper-left corner of the Timeline range. |
| base_field_name | System.String | The name of PivotField in PivotTable.BaseFields |
### Example
```python
# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 10, 5, "date")
```
## add(self, pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Add a new Timeline using PivotTable as data source
### Returns
The new add Timeline index
```python
def add(self, pivot, row, column, base_field_index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Timeline range. |
| column | int | Column index of the cell in the upper-left corner of the Timeline range. |
| base_field_index | int | The index of PivotField in PivotTable.BaseFields |
### Example
```python
# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 15, 5, 1)
```
## add(self, pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Add a new Timeline using PivotTable as data source
### Returns
The new add Timeline index
```python
def add(self, pivot, row, column, base_field):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Timeline range. |
| column | int | Column index of the cell in the upper-left corner of the Timeline range. |
| base_field | aspose.cells.pivot.PivotField | The PivotField in PivotTable.BaseFields |
### Example
```python
# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 20, 5, pivot.base_fields[1])
```
### See Also
* module [`aspose.cells.timelines`](../../)
* class [`TimelineCollection`](/cells/python-net/aspose.cells.timelines/timelinecollection)
