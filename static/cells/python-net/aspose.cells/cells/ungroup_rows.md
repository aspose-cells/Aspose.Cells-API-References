##ungroup_rows method
## ungroup_rows(self, first_index, last_index) {#int-int}
Ungroups rows.
```python
def ungroup_rows(self, first_index, last_index):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| first_index | int | The first row index to be ungrouped. |
| last_index | int | The last row index to be ungrouped. |
### Remarks
Only removes outer group info.
## ungroup_rows(self, first_index, last_index, is_all) {#int-int-bool}
Ungroups rows.
```python
def ungroup_rows(self, first_index, last_index, is_all):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| first_index | int | The first row index to be ungrouped. |
| last_index | int | The last row index to be ungrouped. |
| is_all | bool | True, removes all grouped info.Otherwise, remove the outer group info. |
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
