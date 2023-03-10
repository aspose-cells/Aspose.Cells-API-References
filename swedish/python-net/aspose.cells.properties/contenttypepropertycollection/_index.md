---
title: ContentTypePropertyCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells.properties/contenttypepropertycollection/
is_root: false
---
##  ContentTypePropertyCollection klass
En samling av [ContentTypeProperty](/cells/sv/python-net/aspose.cells.properties/contenttypeproperty) objekt som representerar ytterligare information.



Typen ContentTypePropertyCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add(name, value)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str) | Lägger till egenskapsinformation för innehållstyp.|
| [add(name, value, type)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str-str) | Lägger till egenskapsinformation för innehållstyp.|
| [copy_to(array)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells.properties/contenttypepropertycollection/binary_search/#ContentTypeProperty) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



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
* klass [ContentTypeProperty](/cells/sv/python-net/aspose.cells.properties/contenttypeproperty)
