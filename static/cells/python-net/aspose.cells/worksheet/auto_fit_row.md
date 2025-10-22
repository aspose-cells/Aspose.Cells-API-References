##auto_fit_row method
## auto_fit_row(self, row_index) {#int}
Autofits the row height.
```python
def auto_fit_row(self, row_index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row_index | int | Row index. |
### Remarks
AutoFitRow is an imprecise function.
## auto_fit_row(self, row_index, first_column, last_column) {#int-int-int}
Autofits the row height.
```python
def auto_fit_row(self, row_index, first_column, last_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row_index | int | Row index. |
| first_column | int | First column index. |
| last_column | int | Last column index. |
### Remarks
This method autofits a row based on content in a range of cells within the row.
## auto_fit_row(self, row_index, first_column, last_column, options) {#int-int-int-aspose.cells.AutoFitterOptions}
Autofits the row height.
```python
def auto_fit_row(self, row_index, first_column, last_column, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row_index | int | Row index. |
| first_column | int | First column index. |
| last_column | int | Last column index. |
| options | aspose.cells.AutoFitterOptions | The auto fitter options |
### Remarks
This method autofits a row based on content in a range of cells within the row.
## auto_fit_row(self, start_row, end_row, start_column, end_column) {#int-int-int-int}
Autofits row height in a rectangle range.
```python
def auto_fit_row(self, start_row, end_row, start_column, end_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start_row | int | Start row index. |
| end_row | int | End row index. |
| start_column | int | Start column index. |
| end_column | int | End column index. |
### See Also
* module [`aspose.cells`](../../)
* class [`Worksheet`](/cells/python-net/aspose.cells/worksheet)
