---
title: WorksheetCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1630
url: /sv/python-net/aspose.cells/worksheetcollection/
is_root: false
---
##  WorksheetCollection klass
Kapslar in en samling av [Worksheet](/cells/sv/python-net/aspose.cells/worksheet) objekt.



Typen WorksheetCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [web_extension_task_panes](/cells/sv/python-net/aspose.cells/worksheetcollection/web_extension_task_panes) | Hämtar listan med uppgiftsrutor.|
| [web_extensions](/cells/sv/python-net/aspose.cells/worksheetcollection/web_extensions) | Hämtar listan med uppgiftsrutor.|
| [threaded_comment_authors](/cells/sv/python-net/aspose.cells/worksheetcollection/threaded_comment_authors) | Hämtar listan över trådade kommentarsförfattare.|
| [is_refresh_all_connections](/cells/sv/python-net/aspose.cells/worksheetcollection/is_refresh_all_connections) | Anger om uppdatera alla anslutningar vid öppning av fil i MS Excel.|
| [names](/cells/sv/python-net/aspose.cells/worksheetcollection/names) | Hämtar samlingen av alla namnobjekt i kalkylarket.|
| [active_sheet_name](/cells/sv/python-net/aspose.cells/worksheetcollection/active_sheet_name) | Representerar namnet på det aktiva kalkylbladet när kalkylarket öppnas.|
| [active_sheet_index](/cells/sv/python-net/aspose.cells/worksheetcollection/active_sheet_index) | Representerar indexet för aktivt kalkylblad när kalkylarket öppnas.|
| [dxfs](/cells/sv/python-net/aspose.cells/worksheetcollection/dxfs) | Hämtar master differentialformateringsposter.|
| [xml_maps](/cells/sv/python-net/aspose.cells/worksheetcollection/xml_maps) | Hämtar och ställer in XML-kartorna i arbetsboken.|
| [built_in_document_properties](/cells/sv/python-net/aspose.cells/worksheetcollection/built_in_document_properties) | Returnerar en [DocumentProperty](/cells/sv/python-net/aspose.cells.properties/documentproperty)-samling som representerar alla inbyggda dokumentegenskaper i kalkylarket.|
| [custom_document_properties](/cells/sv/python-net/aspose.cells/worksheetcollection/custom_document_properties) | Returnerar en [DocumentProperty](/cells/sv/python-net/aspose.cells.properties/documentproperty)-samling som representerar alla anpassade dokumentegenskaper i kalkylarket.|
| [ole_size](/cells/sv/python-net/aspose.cells/worksheetcollection/ole_size) | Hämtar och ställer in den visade storleken när arbetsboksfilen används som ett Ole-objekt.|
| [external_links](/cells/sv/python-net/aspose.cells/worksheetcollection/external_links) | Representerar externa länkar i en arbetsbok.|
| [table_styles](/cells/sv/python-net/aspose.cells/worksheetcollection/table_styles) | Får [WorksheetCollection.table_styles](/cells/sv/python-net/aspose.cells/worksheetcollection#table_styles) objekt.|
| [revision_logs](/cells/sv/python-net/aspose.cells/worksheetcollection/revision_logs) |Representerar revisionsloggar.|
| [capacity](/cells/sv/python-net/aspose.cells/worksheetcollection/capacity) | Hämtar eller ställer in antalet element som arraylistan kan innehålla.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [get(index)](/cells/sv/python-net/aspose.cells/worksheetcollection/get/#int) |Lägg till API for Python Via .Net.eftersom detta [int index] inte stöds|
| [get(sheet_name)](/cells/sv/python-net/aspose.cells/worksheetcollection/get/#str) | Lägg till API for Python Via .Net.eftersom detta [strängarknamn] inte stöds|
| [add(type)](/cells/sv/python-net/aspose.cells/worksheetcollection/add/#SheetType) | Lägger till ett kalkylblad i samlingen.|
| [add()](/cells/sv/python-net/aspose.cells/worksheetcollection/add/#) | Lägger till ett kalkylblad i samlingen.|
| [add(sheet_name)](/cells/sv/python-net/aspose.cells/worksheetcollection/add/#str) | Lägger till ett kalkylblad i samlingen.|
| [register_add_in_function(add_in_file, function_name, lib)](/cells/sv/python-net/aspose.cells/worksheetcollection/register_add_in_function/#str-str-bool) | Lägger till tilläggsfunktion i arbetsboken|
| [register_add_in_function(id, function_name)](/cells/sv/python-net/aspose.cells/worksheetcollection/register_add_in_function/#int-str) | Lägger till tilläggsfunktion i arbetsboken|
| [add_copy(sheet_name)](/cells/sv/python-net/aspose.cells/worksheetcollection/add_copy/#str) | Lägger till ett kalkylblad till samlingen och kopierar data från ett befintligt kalkylblad.|
| [add_copy(sheet_index)](/cells/sv/python-net/aspose.cells/worksheetcollection/add_copy/#int) | Lägger till ett kalkylblad till samlingen och kopierar data från ett befintligt kalkylblad.|
| [get_range_by_name(range_name)](/cells/sv/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str) | Hämtar Range-objekt med fördefinierat namn.|
| [get_range_by_name(range_name, current_sheet_index, include_table)](/cells/sv/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str-int-bool) | Får [Range](/cells/sv/python-net/aspose.cells/range) efter fördefinierat namn eller tabellnamn|
| [copy_to(array)](/cells/sv/python-net/aspose.cells/worksheetcollection/copy_to/#list) | Kopierar hela arraylistan till en kompatibel endimensionell arraylista, med början i början av målarraylistan.|
| [copy_to(index, array, array_index, count)](/cells/sv/python-net/aspose.cells/worksheetcollection/copy_to/#int-list-int-int) |Kopierar ett intervall av element från arraylistan till en kompatibel endimensionell arraylista, med början vid det angivna indexet för målarraylistan.|
| [index_of(item, index)](/cells/sv/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som sträcker sig från det angivna indexet till det sista elementet.|
| [index_of(item, index, count)](/cells/sv/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den första förekomsten inom intervallet av element i arraylistan som börjar vid det angivna indexet och innehåller det angivna antalet element.|
| [last_index_of(item)](/cells/sv/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom hela arraylistan.|
| [last_index_of(item, index)](/cells/sv/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int) | Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som sträcker sig från det första elementet till det angivna indexet.|
| [last_index_of(item, index, count)](/cells/sv/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int-int) |Söker efter det angivna objektet och returnerar det nollbaserade indexet för den senaste förekomsten inom intervallet av element i arraylistan som innehåller det angivna antalet element och slutar vid det angivna indexet.|
| [create_range(address, sheet_index)](/cells/sv/python-net/aspose.cells/worksheetcollection/create_range/#str-int) | Skapar ett [Range](/cells/sv/python-net/aspose.cells/range)-objekt från en adress i intervallet.|
| [create_union_range(address, sheet_index)](/cells/sv/python-net/aspose.cells/worksheetcollection/create_union_range/#str-int) | Skapar ett [Range](/cells/sv/python-net/aspose.cells/range)-objekt från en adress i intervallet.|
| [get_sheet_by_code_name(code_name)](/cells/sv/python-net/aspose.cells/worksheetcollection/get_sheet_by_code_name/#str) | Hämtar kalkylbladet med kodnamnet.|
| [sort_names()](/cells/sv/python-net/aspose.cells/worksheetcollection/sort_names/#) | Sorterar de definierade namnen.|
| [swap_sheet(sheet_index1, sheet_index2)](/cells/sv/python-net/aspose.cells/worksheetcollection/swap_sheet/#int-int) | Byter de två arken.|
| [remove_at(name)](/cells/sv/python-net/aspose.cells/worksheetcollection/remove_at/#str) | Tar bort elementet med ett angivet namn.|
| [get_named_ranges()](/cells/sv/python-net/aspose.cells/worksheetcollection/get_named_ranges/#) | Hämtar alla fördefinierade namngivna intervall i kalkylarket.|
| [get_named_ranges_and_tables()](/cells/sv/python-net/aspose.cells/worksheetcollection/get_named_ranges_and_tables/#) | Hämtar alla fördefinierade namngivna intervall i kalkylarket.|
| [set_ole_size(start_row, end_row, start_column, end_column)](/cells/sv/python-net/aspose.cells/worksheetcollection/set_ole_size/#int-int-int-int) | Ställer in visad storlek när arbetsboksfil används som ett Ole-objekt.|
| [clear_pivottables()](/cells/sv/python-net/aspose.cells/worksheetcollection/clear_pivottables/#) | Rensar pivottabeller från kalkylarket.|
| [refresh_pivot_tables()](/cells/sv/python-net/aspose.cells/worksheetcollection/refresh_pivot_tables/#) | Uppdaterar alla pivottabeller i WorksheetCollection.|
| [binary_search(item)](/cells/sv/python-net/aspose.cells/worksheetcollection/binary_search/#Worksheet) | Söker i hela den sorterade arraylistan efter ett element med hjälp av standardjämföraren och returnerar elementets nollbaserade index.|



###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook()
sheets = workbook.worksheets
# Add a worksheet
sheets.add()
# Change the name of a worksheet
sheets[0].name = "First Sheet"
# Set the active sheet to the second worksheet
sheets.active_sheet_index = 1

```

###  Se även
* modul [aspose.cells](..)
* klass [DocumentProperty](/cells/sv/python-net/aspose.cells.properties/documentproperty)
* klass [Range](/cells/sv/python-net/aspose.cells/range)
* klass [Worksheet](/cells/sv/python-net/aspose.cells/worksheet)
