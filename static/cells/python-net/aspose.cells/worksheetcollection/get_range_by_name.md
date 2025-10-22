##get_range_by_name method
## get_range_by_name(self, range_name) {#System.String}
Gets Range object by pre-defined name.
### Returns
Range object.
Returns null if the named range does not exist.
```python
def get_range_by_name(self, range_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| range_name | System.String | Name of range. |
## get_range_by_name(self, range_name, current_sheet_index, include_table) {#System.String-int-bool}
Gets [`Range`](/cells/python-net/aspose.cells/range) by pre-defined name or table's name
### Returns
```python
def get_range_by_name(self, range_name, current_sheet_index, include_table):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| range_name | System.String | Name of range or table's name. |
| current_sheet_index | int | The sheet index. -1 represents global . |
| include_table | bool | Indicates whether checking all tables. |
### See Also
* module [`aspose.cells`](../../)
* class [`Range`](/cells/python-net/aspose.cells/range)
* class [`WorksheetCollection`](/cells/python-net/aspose.cells/worksheetcollection)
