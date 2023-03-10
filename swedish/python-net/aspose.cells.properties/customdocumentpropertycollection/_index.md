---
title: CustomDocumentPropertyCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells.properties/customdocumentpropertycollection/
is_root: false
---
##  CustomDocumentPropertyCollection klass
En samling anpassade dokumentegenskaper.



**Arv:** [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) → 
[DocumentPropertyCollection](/cells/sv/python-net/aspose.cells.properties/documentpropertycollection)



Typen CustomDocumentPropertyCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [capacity](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [index_of(name)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#str) | Hämtar indexet för en egenskap efter namn.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [copy_to(array)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [add(name, value)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-str) | Skapar en ny anpassad dokumentegenskap för**PropertyType.String** data typ.|
| [add(name, value)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-int) | Skapar en ny anpassad dokumentegenskap för**PropertyType.Number** data typ.|
| [add(name, value)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-DateTime) | Skapar en ny anpassad dokumentegenskap för**PropertyType.DateTime** data typ.|
| [add(name, value)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-bool) | Skapar en ny anpassad dokumentegenskap för**PropertyType.Boolean** data typ.|
| [add(name, value)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-float) | Skapar en ny anpassad dokumentegenskap för**PropertyType.Float** data typ.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/binary_search/#DocumentProperty) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|
| [add_link_to_content(name, source)](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/add_link_to_content/#str-str) | Skapar en ny anpassad dokumentegenskap som länkar till innehåll.|
| [update_linked_property_value()](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_property_value/#) |Uppdatera anpassat dokumentegenskapsvärde som länkar till innehåll.|
| [update_linked_range()](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_range/#) | Uppdatera anpassat dokumentegenskapsvärde till länkat intervall.|



###  Anmärkningar

Varje [DocumentProperty](/cells/sv/python-net/aspose.cells.properties/documentproperty)-objekt representerar en anpassad egenskap för ett containerdokument.

###  Exempel

```python
from aspose.cells import Workbook

# Instantiate a Workbook object
workbook = Workbook("book1.xls")
# Retrieve a list of all custom document properties of the Excel file
customProperties = workbook.worksheets.custom_document_properties

```

###  Se även
* modul [aspose.cells.properties](..)
* klass [CustomDocumentPropertyCollection](/cells/sv/python-net/aspose.cells.properties/customdocumentpropertycollection)
* klass [DocumentProperty](/cells/sv/python-net/aspose.cells.properties/documentproperty)
* klass [DocumentPropertyCollection](/cells/sv/python-net/aspose.cells.properties/documentpropertycollection)
