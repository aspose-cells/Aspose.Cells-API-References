---
title: add метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---
##  add(url) {#str}
Добавьте [XmlMap](/cells/ru/python-net/aspose.cells/xmlmap) по URL-адресу/пути файла xml/xsd.


###  Возвращает

[XmlMap](/cells/ru/python-net/aspose.cells/xmlmap) индекс объекта.


```python
def add(self, url):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| url | str | URL-адрес/путь файла xml/xsd.|

###  Пример

Следующий код добавляет две карты XmlMaps с помощью файла xsd и файла xml.

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



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [XmlMap](/cells/ru/python-net/aspose.cells/xmlmap)
* класс [XmlMapCollection](/cells/ru/python-net/aspose.cells/xmlmapcollection)
