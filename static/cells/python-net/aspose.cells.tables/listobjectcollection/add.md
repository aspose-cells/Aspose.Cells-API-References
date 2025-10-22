##add method
## add(self, start_cell, end_cell, has_headers) {#System.String-System.String-bool}
Adds a ListObject to the worksheet.
### Returns
The index of the new ListObject
```python
def add(self, start_cell, end_cell, has_headers):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start_cell | System.String | The start cell of the list range. |
| end_cell | System.String | The end cell of the list range. |
| has_headers | bool | Whether the range has headers. |
## add(self, start_row, start_column, end_row, end_column, has_headers) {#int-int-int-int-bool}
Adds a ListObject to the worksheet.
### Returns
The index of the new ListObject
```python
def add(self, start_row, start_column, end_row, end_column, has_headers):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start_row | int | The start row of the list range. |
| start_column | int | The start row of the list range. |
| end_row | int | The start row of the list range. |
| end_column | int | The start row of the list range. |
| has_headers | bool | Whether the range has headers. |
### See Also
* module [`aspose.cells.tables`](../../)
* class [`ListObjectCollection`](/cells/python-net/aspose.cells.tables/listobjectcollection)
