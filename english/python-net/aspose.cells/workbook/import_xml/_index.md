---
title: import_xml method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 220
url: /python-net/aspose.cells/workbook/import_xml/
is_root: false
---

## import_xml(url, sheet_name, row, col) {#str-str-int-int}

Imports/Updates an XML data file into the workbook.



```python
def import_xml(self, url, sheet_name, row, col):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| url | str | the url/path of the xml file. |
| sheet_name | str | the destination sheet name. |
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


## import_xml(stream, sheet_name, row, col) {#io.RawIOBase-str-int-int}

Imports/Updates an XML data file into the workbook.



```python
def import_xml(self, stream, sheet_name, row, col):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | the xml file stream. |
| sheet_name | str | the destination sheet name. |
| row | int | the destination row. |
| col | int | the destination column. |



### See Also
* module [aspose.cells](../../)
* class [Workbook](/cells/python-net/aspose.cells/workbook)
