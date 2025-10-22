##create_safe_sheet_name method
## create_safe_sheet_name(, name_proposal) {#System.String}
Checks given sheet name and create a valid one when needed.
If given sheet name conforms to the rules of excel sheet name, then return it.
Otherwise string will be truncated if length exceeds the limit
and invalid characters will be replaced with ' ', then return the rebuilt string value.
### Returns
```python
@staticmethod
def create_safe_sheet_name(name_proposal):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| name_proposal | System.String | sheet name to be used |
## create_safe_sheet_name(, name_proposal, replace_char) {#System.String-System.Char}
Checks given sheet name and create a valid one when needed.
If given sheet name conforms to the rules of excel sheet name, then return it.
Otherwise string will be truncated if length exceeds the limit
and invalid characters will be replaced with given character, then return the rebuilt string value.
### Returns
```python
@staticmethod
def create_safe_sheet_name(name_proposal, replace_char):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| name_proposal | System.String | sheet name to be used |
| replace_char | System.Char | character which will be used to replace invalid characters in given sheet name |
### See Also
* module [`aspose.cells`](../../)
* class [`CellsHelper`](/cells/python-net/aspose.cells/cellshelper)
