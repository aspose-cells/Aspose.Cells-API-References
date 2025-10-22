##SheetSet constructor
## \_\_init\_\_(self, sheet_indexes) {#list}
Creates a sheet set based on exact sheet indexes.
```python
def __init__(self, sheet_indexes):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| sheet_indexes | list | zero based sheet indexes. |
### Remarks
If a sheet is encountered that is not in the workbook, an exception will be thrown during rendering.
## \_\_init\_\_(self, sheet_names) {#list}
Creates a sheet set based on exact sheet names.
```python
def __init__(self, sheet_names):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| sheet_names | list | sheet names. |
### Remarks
If a sheet is encountered that is not in the workbook, an exception will be thrown during rendering.
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`SheetSet`](/cells/python-net/aspose.cells.rendering/sheetset)
