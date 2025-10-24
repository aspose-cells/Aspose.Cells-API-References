##extension_to_save_format method
## extension_to_save_format(, extension) {#System.String}
Converts a file name extension into a SaveFormat value.
### Returns
```python
@staticmethod
def extension_to_save_format(extension):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| extension | System.String | The file extension. Can be with or without a leading dot. Case-insensitive. |
### Remarks
If the extension cannot be recognized, returns [`SaveFormat.UNKNOWN`](/cells/python-net/aspose.cells/saveformat#UNKNOWN).
### See Also
* module [`aspose.cells`](../../)
* class [`FileFormatUtil`](/cells/python-net/aspose.cells/fileformatutil)
* class [`SaveFormat`](/cells/python-net/aspose.cells/saveformat)
