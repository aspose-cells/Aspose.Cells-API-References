---
title: add method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---

## add(url) {#str}

Add a [XmlMap](/cells/python-net/aspose.cells/xmlmap) by the url/path of a xml/xsd file.


### Returns 


[XmlMap](/cells/python-net/aspose.cells/xmlmap) object index.


```python
def add(self, url):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| url | str | url/path of a xml/xsd file. |

### Example 


The following code adds two XmlMaps by a xsd file and a xml file.

```python
from aspose.cells import Workbook

wb = Workbook()
xmlMapCollection = wb.worksheets.xml_maps
# Add a XmlMap by a xsd file.
xmlMapCollection.add("schema.xsd")
# Add a XmlMap by a xml file.
xmlMapCollection.add("xml.xml")
wb.save("twoXmlMaps.xlsx")

```



### See Also
* module [aspose.cells](../../)
* class [XmlMapCollection](/cells/python-net/aspose.cells/xmlmapcollection)
