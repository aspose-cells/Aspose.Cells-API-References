##remove_area method
## remove_area(self, index) {#int}
Removes conditional formatted cell range by index.
```python
def remove_area(self, index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| index | int | The index of the conditional formatted cell range to be removed. |
## remove_area(self, start_row, start_column, total_rows, total_columns) {#int-int-int-int}
Remove conditional formatting int the range.
### Returns
Returns TRUE, this FormatCondtionCollection should be removed.
```python
def remove_area(self, start_row, start_column, total_rows, total_columns):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start_row | int | The startRow of the range. |
| start_column | int | The startColumn of the range. |
| total_rows | int | The number of rows of the range. |
| total_columns | int | The number of columns of the range. |
### See Also
* module [`aspose.cells`](../../)
* class [`FormatConditionCollection`](/cells/python-net/aspose.cells/formatconditioncollection)
