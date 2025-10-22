##export_xml method
## export_xml(self, map_name, path) {#System.String-System.String}
Export XML data linked by the specified XML map.
```python
def export_xml(self, map_name, path):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| map_name | System.String | name of the XML map that need to be exported |
| path | System.String | the export path |
### Example
The following code exported the data linked by the first XmlMap.
```python
from aspose.cells import Workbook
wb = Workbook("Book1.xlsx")
# Make sure that the source xlsx file contains a XmlMap.
xmlMap = wb.worksheets.xml_maps[0]
wb.export_xml(xmlMap.name, "output.xml")
```
## export_xml(self, map_name, stream) {#System.String-io.RawIOBase}
Export XML data.
```python
def export_xml(self, map_name, stream):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| map_name | System.String | name of the XML map that need to be exported |
| stream | io.RawIOBase | the export stream |
### See Also
* module [`aspose.cells`](../../)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
