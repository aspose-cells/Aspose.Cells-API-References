##merge_files method
## merge_files(, files, cached_file, dest_file) {#list-System.String-System.String}
Merges some large xls files to a xls file.
```python
@staticmethod
def merge_files(files, cached_file, dest_file):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| files | list | The files. |
| cached_file | System.String | The cached file. |
| dest_file | System.String | The dest file. |
### Remarks
This method only supports merging data, style and formulas to the new file.
The cached file is used to store some temporary data.
### See Also
* module [`aspose.cells`](../../)
* class [`CellsHelper`](/cells/python-net/aspose.cells/cellshelper)
