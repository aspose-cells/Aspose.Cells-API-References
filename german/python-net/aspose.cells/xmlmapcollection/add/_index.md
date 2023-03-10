---
title: add Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---
##  add(url) {#str}
Fügen Sie eine [XmlMap](/cells/de/python-net/aspose.cells/xmlmap) neben der URL/dem Pfad einer xml/xsd-Datei hinzu.


###  Kehrt zurück

[XmlMap](/cells/de/python-net/aspose.cells/xmlmap) Objektindex.


```python
def add(self, url):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| url | str | URL/Pfad einer xml/xsd-Datei.|

###  Beispiel

Der folgende Code fügt zwei XmlMaps durch eine xsd-Datei und eine xml-Datei hinzu.

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



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [XmlMap](/cells/de/python-net/aspose.cells/xmlmap)
* Klasse [XmlMapCollection](/cells/de/python-net/aspose.cells/xmlmapcollection)
