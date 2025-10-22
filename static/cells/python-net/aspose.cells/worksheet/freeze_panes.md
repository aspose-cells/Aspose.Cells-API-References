##freeze_panes method
## freeze_panes(self, cell_name, freezed_rows, freezed_columns) {#System.String-int-int}
Freezes panes at the specified cell in the worksheet.
```python
def freeze_panes(self, cell_name, freezed_rows, freezed_columns):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cell_name | System.String | Cell name. |
| freezed_rows | int | Number of visible rows in top pane, no more than row index. |
| freezed_columns | int | Number of visible columns in left pane, no more than column index. |
### Remarks
Row index and column index cannot all be zero. Number of rows and number of columns
also cannot all be zero.
## freeze_panes(self, row, column, freezed_rows, freezed_columns) {#int-int-int-int}
Freezes panes at the specified cell in the worksheet.
```python
def freeze_panes(self, row, column, freezed_rows, freezed_columns):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | int | Row index. |
| column | int | Column index. |
| freezed_rows | int | Number of visible rows in top pane, no more than row index. |
| freezed_columns | int | Number of visible columns in left pane, no more than column index. |
### Remarks
Row index and column index cannot all be zero. Number of rows and number of columns
also cannot all be zero.
The first two parameters specify the froze position and the last two parameters specify the area frozen on the left top pane.
### See Also
* module [`aspose.cells`](../../)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)
