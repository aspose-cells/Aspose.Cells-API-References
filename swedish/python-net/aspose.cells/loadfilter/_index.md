---
title: LoadFilter klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1010
url: /sv/python-net/aspose.cells/loadfilter/
is_root: false
---
##  LoadFilter klass
Representerar filtret som ger alternativ för att ladda data när du laddar arbetsbok från mall.



Typen LoadFilter avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [LoadFilter()](/cells/sv/python-net/aspose.cells/loadfilter/__init__/#) | Konstruerar ett LoadFilter med standardfilteralternativ LoadDataFilterOptions.All.|
| [LoadFilter(opts)](/cells/sv/python-net/aspose.cells/loadfilter/__init__/#LoadDataFilterOptions) | Konstruerar ett LoadFilter med givna filteralternativ.|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [load_data_filter_options](/cells/sv/python-net/aspose.cells/loadfilter/load_data_filter_options) | Filteralternativen för att ange vilken data som ska laddas.|
| [sheets_in_loading_order](/cells/sv/python-net/aspose.cells/loadfilter/sheets_in_loading_order) | Anger ark(index) och ordning som ska laddas.<br/>Standard är null, vilket anger att alla ark ska laddas i standardordningen i mallfilen.<br/> Om inte null och vissa arks index inte finns i den returnerade arrayen, kommer arket inte att laddas.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [start_sheet(sheet)](/cells/sv/python-net/aspose.cells/loadfilter/start_sheet/#Worksheet) | Förbereder filteralternativ innan du laddar ett visst kalkylblad.<br/>Användarens implementering av LoadFilter kan ändra LoadDataFilterOptions här<br/> för att ange hur man laddar data för detta kalkylblad.|



###  Anmärkningar

Användaren kan specificera filteralternativen eller implementera sin egen LoadFilter för att specificera hur data ska laddas.

###  Se även
* modul [aspose.cells](..)
