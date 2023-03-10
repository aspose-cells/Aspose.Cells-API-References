---
title: metodo add
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---
##  add(url) {#str}
Aggiungere un [XmlMap](/cells/it/python-net/aspose.cells/xmlmap) dall'URL/percorso di un file xml/xsd.


###  ritorna

[XmlMap](/cells/it/python-net/aspose.cells/xmlmap) indice oggetto.


```python
def add(self, url):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| url | str | url/percorso di un file xml/xsd.|

###  Esempio

Il codice seguente aggiunge due XmlMap tramite un file xsd e un file xml.

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



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [XmlMap](/cells/it/python-net/aspose.cells/xmlmap)
* classe [XmlMapCollection](/cells/it/python-net/aspose.cells/xmlmapcollection)
