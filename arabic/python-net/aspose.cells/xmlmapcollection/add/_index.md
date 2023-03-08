---
title: طريقة add
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---
##  add(url) {#str}
أضف [XmlMap](/cells/ar/python-net/aspose.cells/xmlmap) عن طريق عنوان url / مسار ملف xml / xsd.


###  عائدات

[XmlMap](/cells/ar/python-net/aspose.cells/xmlmap) فهرس العنصر.


```python
def add(self, url):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| url | str | عنوان url / مسار ملف xml / xsd.|

###  مثال

تضيف التعليمة البرمجية التالية خبقتين XmlMaps بواسطة ملف xsd وملف xml.

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



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [XmlMap](/cells/ar/python-net/aspose.cells/xmlmap)
* فئة [XmlMapCollection](/cells/ar/python-net/aspose.cells/xmlmapcollection)
