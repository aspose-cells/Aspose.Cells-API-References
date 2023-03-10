---
title: ContentTypeProperty klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 20
url: /sv/python-net/aspose.cells.properties/contenttypeproperty/
is_root: false
---
##  ContentTypeProperty klass
Representerar identifieringsinformation.



Typen ContentTypeProperty avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [name](/cells/sv/python-net/aspose.cells.properties/contenttypeproperty/name) | Returnerar eller anger namnet på objektet.|
| [value](/cells/sv/python-net/aspose.cells.properties/contenttypeproperty/value) | Returnerar eller ställer in värdet för innehållstypsegenskapen.|
| [type](/cells/sv/python-net/aspose.cells.properties/contenttypeproperty/type) | Hämtar och ställer in typ av fastighet.|
| [is_nillable](/cells/sv/python-net/aspose.cells.properties/contenttypeproperty/is_nillable) | Indikerar om värdet kan vara tomt.|



###  Exempel

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Se även
* modul [aspose.cells.properties](..)
