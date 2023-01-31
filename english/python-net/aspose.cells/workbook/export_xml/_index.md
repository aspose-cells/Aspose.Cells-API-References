---
title: export_xml method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 140
url: /python-net/aspose.cells/workbook/export_xml/
is_root: false
---

## export_xml(map_name, path) {#str-str}

Export XML data linked by the specified XML map.



```python
def export_xml(self, map_name, path):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| map_name | str | name of the XML map that need to be exported |
| path | str | the export path |
### Example 


The following code exported the data linked by the first XmlMap.

```
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")

# Make sure that the source xlsx file contains a XmlMap.
xmlMap = wb.worksheets.xml_maps[0]
wb.export_xml(xmlMap.name, "output.xml")

```


## export_xml(map_name, stream) {#str-io.RawIOBase}

Export XML data.



```python
def export_xml(self, map_name, stream):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| map_name | str | name of the XML map that need to be exported |
| stream | io.RawIOBase | the export stream |



### See Also
* module [aspose.cells](../../)
* class [Workbook](/cells/python-net/aspose.cells/workbook)
