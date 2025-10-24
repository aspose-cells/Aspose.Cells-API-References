##merge method
## merge(self, first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Merges a specified range of cells into a single cell.
```python
def merge(self, first_row, first_column, total_rows, total_columns):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| first_row | int | First row of this range(zero based) |
| first_column | int | First column of this range(zero based) |
| total_rows | int | Number of rows(one based) |
| total_columns | int | Number of columns(one based) |
### Remarks
Reference the merged cell via the address of the upper-left cell in the range.
## merge(self, first_row, first_column, total_rows, total_columns, merge_conflict) {#int-int-int-int-bool}
Merges a specified range of cells into a single cell.
```python
def merge(self, first_row, first_column, total_rows, total_columns, merge_conflict):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| first_row | int | First row of this range(zero based) |
| first_column | int | First column of this range(zero based) |
| total_rows | int | Number of rows(one based) |
| total_columns | int | Number of columns(one based) |
| merge_conflict | bool | Merge conflict merged ranges. |
### Remarks
Reference the merged cell via the address of the upper-left cell in the range.
If mergeConflict is true and the merged range conflicts with other merged cells,
other merged cells will be  automatically removed.
## merge(self, first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict) {#int-int-int-int-bool-bool}
Merges a specified range of cells into a single cell.
```python
def merge(self, first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| first_row | int | First row of this range(zero based) |
| first_column | int | First column of this range(zero based) |
| total_rows | int | Number of rows(one based) |
| total_columns | int | Number of columns(one based) |
| check_conflict | bool | Indicates whether check the merged cells intersects other merged cells |
| merge_conflict | bool | Merge conflict merged ranges. |
### Remarks
Reference the merged cell via the address of the upper-left cell in the range.
If mergeConflict is true and the merged range conflicts with other merged cells,
other merged cells will be  automatically removed.
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
