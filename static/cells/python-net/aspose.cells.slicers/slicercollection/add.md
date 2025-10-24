##add method
## add(self, pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-System.String-System.String}
Add a new Slicer using PivotTable as data source
### Returns
The new add Slicer index
```python
def add(self, pivot, dest_cell_name, base_field_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| dest_cell_name | System.String | The cell in the upper-left corner of the Slicer range. |
| base_field_name | System.String | The name of PivotField in PivotTable.BaseFields |
### Example
```python
slicers.add(pivot, "E3", "fruit")
```
## add(self, pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-System.String-int}
Add a new Slicer using PivotTable as data source
### Returns
The new add Slicer index
```python
def add(self, pivot, dest_cell_name, base_field_index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| dest_cell_name | System.String | The cell in the upper-left corner of the Slicer range. |
| base_field_index | int | The index of PivotField in PivotTable.BaseFields |
### Example
```python
slicers.add(pivot, "E20", 0)
```
## add(self, pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-System.String-aspose.cells.pivot.PivotField}
Add a new Slicer using PivotTable as data source
### Returns
The new add Slicer index
```python
def add(self, pivot, dest_cell_name, base_field):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| dest_cell_name | System.String | The cell in the upper-left corner of the Slicer range. |
| base_field | aspose.cells.pivot.PivotField | The PivotField in PivotTable.BaseFields |
### Example
```python
slicers.add(pivot, "I3", pivot.base_fields[0])
```
## add(self, table, index, dest_cell_name) {#aspose.cells.tables.ListObject-int-System.String}
Add a new Slicer using ListObjet as data source
### Returns
The new add Slicer index
```python
def add(self, table, index, dest_cell_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | ListObject object |
| index | int | The index of ListColumn in ListObject.ListColumns |
| dest_cell_name | System.String | The cell in the upper-left corner of the Slicer range. |
### Example
```python
slicers.add(table, 1, "E38")
```
## add(self, table, list_column, dest_cell_name) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-System.String}
Add a new Slicer using ListObjet as data source
### Returns
The new add Slicer index
```python
def add(self, table, list_column, dest_cell_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | ListObject object |
| list_column | aspose.cells.tables.ListColumn | The ListColumn in ListObject.ListColumns |
| dest_cell_name | System.String | The cell in the upper-left corner of the Slicer range. |
### Example
```python
slicers.add(table, table.list_columns[1], "I38")
```
## add(self, pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-System.String}
Add a new Slicer using PivotTable as data source
### Returns
The new add Slicer index
```python
def add(self, pivot, row, column, base_field_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
| base_field_name | System.String | The name of PivotField in PivotTable.BaseFields |
### Example
```python
slicers.add(pivot, 20, 12, "fruit")
```
## add(self, pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Add a new Slicer using PivotTable as data source
### Returns
The new add Slicer index
```python
def add(self, pivot, row, column, base_field_index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
| base_field_index | int | The index of PivotField in PivotTable.BaseFields |
### Example
```python
slicers.add(pivot, 20, 8, 0)
```
## add(self, pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Add a new Slicer using PivotTable as data source
### Returns
The new add Slicer index
```python
def add(self, pivot, row, column, base_field):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | PivotTable object |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
| base_field | aspose.cells.pivot.PivotField | The PivotField in PivotTable.BaseFields |
### Example
```python
slicers.add(pivot, 3, 12, pivot.base_fields[0])
```
## add(self, table, list_column, row, column) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int}
Add a new Slicer using ListObjet as data source
### Returns
The new add Slicer index
```python
def add(self, table, list_column, row, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | ListObject object |
| list_column | aspose.cells.tables.ListColumn | The ListColumn in ListObject.ListColumns |
| row | int | Row index of the cell in the upper-left corner of the Slicer range. |
| column | int | Column index of the cell in the upper-left corner of the Slicer range. |
### Example
```python
slicers.add(table, table.list_columns[1], 38, 12)
```
### See Also
* module [`aspose.cells.slicers`](../../)
* class [`SlicerCollection`](/cells/python-net/aspose.cells.slicers/slicercollection)
