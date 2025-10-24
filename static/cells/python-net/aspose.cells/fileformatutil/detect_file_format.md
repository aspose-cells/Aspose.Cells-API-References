##detect_file_format method
## detect_file_format(, stream) {#io.RawIOBase}
Detects and returns the information about a format of an excel stored in a stream.
### Returns
A [`FileFormatInfo`](/cells/python-net/aspose.cells/fileformatinfo) object that contains the detected information.
```python
@staticmethod
def detect_file_format(stream):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase |  |
## detect_file_format(, file_path) {#System.String}
Detects and returns the information about a format of an excel stored in a file.
### Returns
A [`FileFormatInfo`](/cells/python-net/aspose.cells/fileformatinfo) object that contains the detected information.
```python
@staticmethod
def detect_file_format(file_path):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file_path | System.String | The file path. |
## detect_file_format(, stream, password) {#io.RawIOBase-System.String}
Detects and returns the information about a format of an excel stored in a stream.
### Returns
A [`FileFormatInfo`](/cells/python-net/aspose.cells/fileformatinfo) object that contains the detected information.
```python
@staticmethod
def detect_file_format(stream, password):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase |  |
| password | System.String | The password for encrypted ooxml files. |
## detect_file_format(, file_path, password) {#System.String-System.String}
Detects and returns the information about a format of an excel stored in a file.
### Returns
A [`FileFormatInfo`](/cells/python-net/aspose.cells/fileformatinfo) object that contains the detected information.
```python
@staticmethod
def detect_file_format(file_path, password):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file_path | System.String | The file path. |
| password | System.String | The password for encrypted ooxml files. |
### See Also
* module [`aspose.cells`](../../)
* class [`FileFormatInfo`](/cells/python-net/aspose.cells/fileformatinfo)
* class [`FileFormatUtil`](/cells/python-net/aspose.cells/fileformatutil)
