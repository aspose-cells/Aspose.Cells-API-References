---
title: add yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---
##  add(url) {#str}
Bir xml/xsd dosyasının url/yoluna göre bir [XmlMap](/cells/tr/python-net/aspose.cells/xmlmap) ekleyin.


###  İadeler

[XmlMap](/cells/tr/python-net/aspose.cells/xmlmap) nesne dizini.


```python
def add(self, url):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| url | str | bir xml/xsd dosyasının url/yolu.|

###  örnekler

Aşağıdaki kod, bir xsd dosyası ve bir xml dosyası tarafından iki XmlMaps ekler.

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



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [XmlMap](/cells/tr/python-net/aspose.cells/xmlmap)
* sınıf [XmlMapCollection](/cells/tr/python-net/aspose.cells/xmlmapcollection)
