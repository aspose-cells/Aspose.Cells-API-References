##import_csv method
## import_csv(self, file_name, options, first_row, first_column) {#System.String-aspose.cells.TxtLoadOptions-int-int}
Import a CSV file to the cells.
```python
def import_csv(self, file_name, options, first_row, first_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file_name | System.String | The CSV file name. |
| options | aspose.cells.TxtLoadOptions | The load options for reading text file |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |
## import_csv(self, stream, options, first_row, first_column) {#io.RawIOBase-aspose.cells.TxtLoadOptions-int-int}
Import a CSV file to the cells.
```python
def import_csv(self, stream, options, first_row, first_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The CSV file stream. |
| options | aspose.cells.TxtLoadOptions | The load options for reading text file |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |
## import_csv(self, file_name, splitter, convert_numeric_data, first_row, first_column) {#System.String-System.String-bool-int-int}
Import a CSV file to the cells.
```python
def import_csv(self, file_name, splitter, convert_numeric_data, first_row, first_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| file_name | System.String | The CSV file name. |
| splitter | System.String | The splitter |
| convert_numeric_data | bool | Whether the string in text file is converted to numeric data. |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |
## import_csv(self, stream, splitter, convert_numeric_data, first_row, first_column) {#io.RawIOBase-System.String-bool-int-int}
Import a CSV file to the cells.
```python
def import_csv(self, stream, splitter, convert_numeric_data, first_row, first_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The CSV file stream. |
| splitter | System.String | The splitter |
| convert_numeric_data | bool | Whether the string in text file is converted to numeric data. |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
