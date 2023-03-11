---
title: add méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---
##  add(url) {#str}
Ajoutez un [XmlMap](/cells/fr/python-net/aspose.cells/xmlmap) par l'url/chemin d'un fichier xml/xsd.


###  Retour

[XmlMap](/cells/fr/python-net/aspose.cells/xmlmap) indice d'objet.


```python
def add(self, url):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| url | str | url/chemin d'un fichier xml/xsd.|

###  Exemple

Le code suivant ajoute deux XmlMaps par un fichier xsd et un fichier xml.

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



###  Voir également
* module [aspose.cells](../../)
* classe [XmlMap](/cells/fr/python-net/aspose.cells/xmlmap)
* classe [XmlMapCollection](/cells/fr/python-net/aspose.cells/xmlmapcollection)
