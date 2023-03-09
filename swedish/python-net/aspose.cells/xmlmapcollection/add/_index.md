---
title: add metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---
##  add(url) {#str}
Lägg till ett [XmlMap](/cells/sv/python-net/aspose.cells/xmlmap) med url/sökväg till en xml/xsd-fil.


###  Returnerar

[XmlMap](/cells/sv/python-net/aspose.cells/xmlmap) objektindex.


```python
def add(self, url):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| url | str | url/sökväg till en xml/xsd-fil.|

###  Exempel

Följande kod lägger till två XmlMaps av en xsd-fil och en xml-fil.

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



###  Se även
* modul [aspose.cells](../../)
* klass [XmlMap](/cells/sv/python-net/aspose.cells/xmlmap)
* klass [XmlMapCollection](/cells/sv/python-net/aspose.cells/xmlmapcollection)
