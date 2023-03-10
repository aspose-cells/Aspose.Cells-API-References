---
title: add método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---
##  add(url) {#str}
Agregue un [XmlMap](/cells/es/python-net/aspose.cells/xmlmap) por la url/ruta de un archivo xml/xsd.


###  Devoluciones

[XmlMap](/cells/es/python-net/aspose.cells/xmlmap) índice de objetos.


```python
def add(self, url):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| url | str | url/ruta de un archivo xml/xsd.|

###  Ejemplo

El siguiente código agrega dos XmlMaps por un archivo xsd y un archivo xml.

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



###  Ver también
* módulo [aspose.cells](../../)
* clase [XmlMap](/cells/es/python-net/aspose.cells/xmlmap)
* clase [XmlMapCollection](/cells/es/python-net/aspose.cells/xmlmapcollection)
