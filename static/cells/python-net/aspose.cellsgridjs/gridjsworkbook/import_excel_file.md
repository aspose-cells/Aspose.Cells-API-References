##import_excel_file method
## import_excel_file {#str}
Imports the excel file from the file path.
```python
def import_excel_file(self, file_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file_name | str | The full path of the file. |
## import_excel_file {#str-str}
Imports the excel file from the file path.
```python
def import_excel_file(self, uid, file_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| uid | str | The unique id for the file cache, if set to null,it will be generated automatically. |
| file_name | str | The full path of the file. |
## import_excel_file {#io.RawIOBase-aspose.cellsgridjs.GridLoadFormat}
Imports the excel file from file stream with load format.
```python
def import_excel_file(self, filestream, format):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| filestream | io.RawIOBase | The stream of the excel file . |
| format | [`GridLoadFormat`](/cells/python-net/aspose.cellsgridjs/gridloadformat) | The LoadFormat of the excel file. |
## import_excel_file {#str-str-str}
Imports the excel file from file path and open password.
```python
def import_excel_file(self, uid, file_name, password):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| uid | str | The unique id for the file cache, if set to null,it will be generated automatically. |
| file_name | str | The full path of the file. |
| password | str | The open password  of the excel file.The value can be null If no passowrd is set. |
## import_excel_file {#str-io.RawIOBase-aspose.cellsgridjs.GridLoadFormat}
Imports the excel file from file stream.
```python
def import_excel_file(self, uid, filestream, format):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| uid | str | The unique id for the file cache, if set to null,it will be generated automatically. |
| filestream | io.RawIOBase | The stream of the excel file . |
| format | [`GridLoadFormat`](/cells/python-net/aspose.cellsgridjs/gridloadformat) | The LoadFormat of the excel file. |
## import_excel_file {#io.RawIOBase-aspose.cellsgridjs.GridLoadFormat-str}
Imports the excel file from file stream with load format and open password.
```python
def import_excel_file(self, filestream, format, password):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| filestream | io.RawIOBase | The stream of the excel file . |
| format | [`GridLoadFormat`](/cells/python-net/aspose.cellsgridjs/gridloadformat) | The LoadFormat of the excel file. |
| password | str | The open password  of the excel file.The value can be null If no passowrd is set. |
## import_excel_file {#str-io.RawIOBase-aspose.cellsgridjs.GridLoadFormat-str}
Imports the excel file from  file stream with load format and open password.
```python
def import_excel_file(self, uid, filestream, format, password):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| uid | str | The unique id for the file cache, if set to null,it will be generated automatically. |
| filestream | io.RawIOBase | The stream of the excel file . |
| format | [`GridLoadFormat`](/cells/python-net/aspose.cellsgridjs/gridloadformat) | The LoadFormat of the excel file. |
| password | str | The open password  of the excel file.The value can be null If no passowrd is set |
### See Also
* module [`aspose.cellsgridjs`](../../)
* class [`GridJsWorkbook`](/cells/python-net/aspose.cellsgridjs/gridjsworkbook)
