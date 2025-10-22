##Workbook constructor
## \_\_init\_\_(self) {#}
Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class.
```python
def __init__(self):
...
```
### Remarks
The default file format type is Xlsx. If you want to create other types of files, please use Workbook(FileFormatType).
### Example
The following code shows how to use the Workbook constructor to create and initialize a new instance of the class.
```python
from aspose.cells import Workbook
workbook = Workbook()
```
## \_\_init\_\_(self, file_format_type) {#aspose.cells.FileFormatType}
Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class.
```python
def __init__(self, file_format_type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file_format_type | aspose.cells.FileFormatType | The new file format. |
### Remarks
The default file format type is Excel97To2003.
### Example
The following code shows how to use the Workbook constructor to create and initialize a new instance of the class with various file format type.
```python
from aspose.cells import FileFormatType, Workbook
workbook = Workbook(FileFormatType.XLSX)
```
## \_\_init\_\_(self, file) {#System.String}
Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class and open a file.
```python
def __init__(self, file):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file | System.String | The file name. |
## \_\_init\_\_(self, stream) {#io.RawIOBase}
Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class and open a stream.
```python
def __init__(self, stream):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The stream. |
## \_\_init\_\_(self, file, load_options) {#System.String-aspose.cells.LoadOptions}
Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class and open a file.
```python
def __init__(self, file, load_options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file | System.String | The file name. |
| load_options | aspose.cells.LoadOptions | The load options |
## \_\_init\_\_(self, stream, load_options) {#io.RawIOBase-aspose.cells.LoadOptions}
Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class and open stream.
```python
def __init__(self, stream, load_options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The stream. |
| load_options | aspose.cells.LoadOptions | The load options |
### See Also
* module [`aspose.cells`](../../)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
