##register_add_in_function method
## register_add_in_function(self, id, function_name) {#int-System.String}
Adds addin function into the workbook
### Returns
URL of the addin file which contains addin functions
```python
def register_add_in_function(self, id, function_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| id | int | ID of the data which contains addin functions,
| function_name | System.String | the addin function name |
## register_add_in_function(self, add_in_file, function_name, lib) {#System.String-System.String-bool}
Adds addin function into the workbook
### Returns
ID of the data which contains given addin function
```python
def register_add_in_function(self, add_in_file, function_name, lib):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| add_in_file | System.String | the file contains the addin functions |
| function_name | System.String | the addin function name |
| lib | bool | whether the given addin file is in the directory or sub-directory of Workbook Add-In library.
### See Also
* module [`aspose.cells`](../../)
* class [`WorksheetCollection`](/cells/python-net/aspose.cells/worksheetcollection)
