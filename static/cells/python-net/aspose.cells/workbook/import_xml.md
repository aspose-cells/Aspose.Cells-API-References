##import_xml method
## import_xml(self, url, sheet_name, row, col) {#System.String-System.String-int-int}
Imports/Updates an XML data file into the workbook.
```python
def import_xml(self, url, sheet_name, row, col):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| url | System.String | the url/path of the xml file. |
| sheet_name | System.String | the destination sheet name. |
| row | int | the destination row |
| col | int | the destination column |
### Example
The following code imports xml data into worksheet 'Sheet 1' at Cell A1.
```python
from aspose.cells import Workbook
wb = Workbook("Book1.xlsx")
wb.import_xml("xml.xml", "Sheet1", 0, 0)
wb.save("output.xlsx")
```
## import_xml(self, stream, sheet_name, row, col) {#io.RawIOBase-System.String-int-int}
Imports/Updates an XML data file into the workbook.
```python
def import_xml(self, stream, sheet_name, row, col):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | the xml file stream. |
| sheet_name | System.String | the destination sheet name. |
| row | int | the destination row. |
| col | int | the destination column. |
### See Also
* module [`aspose.cells`](../../)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
