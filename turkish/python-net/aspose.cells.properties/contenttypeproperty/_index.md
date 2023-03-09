---
title: ContentTypeProperty sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.properties/contenttypeproperty/
is_root: false
---
##  ContentTypeProperty sınıfı
Tanımlayıcı bilgileri temsil eder.



ContentTypeProperty türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [name](/cells/tr/python-net/aspose.cells.properties/contenttypeproperty/name) | Nesnenin adını döndürür veya ayarlar.|
| [value](/cells/tr/python-net/aspose.cells.properties/contenttypeproperty/value) | İçerik türü özelliğinin değerini döndürür veya ayarlar.|
| [type](/cells/tr/python-net/aspose.cells.properties/contenttypeproperty/type) | Özelliğin türünü alır ve ayarlar.|
| [is_nillable](/cells/tr/python-net/aspose.cells.properties/contenttypeproperty/is_nillable) | Değerin boş olup olamayacağını gösterir.|



###  örnekler

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Ayrıca bakınız
* modül [aspose.cells.properties](..)
