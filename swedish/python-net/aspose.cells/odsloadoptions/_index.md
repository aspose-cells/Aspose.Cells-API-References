---
title: OdsLoadOptions klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1100
url: /sv/python-net/aspose.cells/odsloadoptions/
is_root: false
---
##  OdsLoadOptions klass
Representerar alternativen för att ladda ods-filen.



**Arv:** [OdsLoadOptions](/cells/python-net/aspose.cells/odsloadoptions) → 
[LoadOptions](/cells/sv/python-net/aspose.cells/loadoptions)



Typen OdsLoadOptions avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [OdsLoadOptions()](/cells/sv/python-net/aspose.cells/odsloadoptions/__init__/#) | Representerar alternativen för att ladda ods-filen.|
| [OdsLoadOptions(type)](/cells/sv/python-net/aspose.cells/odsloadoptions/__init__/#LoadFormat) | Representerar alternativen för att ladda ods-filen.|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [load_format](/cells/sv/python-net/aspose.cells/odsloadoptions/load_format) | Hämtar laddningsformatet.|
| [password](/cells/sv/python-net/aspose.cells/odsloadoptions/password) | Hämtar och ställer in lösenordet för arbetsboken.|
| [parsing_formula_on_open](/cells/sv/python-net/aspose.cells/odsloadoptions/parsing_formula_on_open) | Anger om formeln analyseras när filen läses.|
| [parsing_pivot_cached_records](/cells/sv/python-net/aspose.cells/odsloadoptions/parsing_pivot_cached_records) | Indikerar om tolkar pivotcachade poster när filen laddas.<br/> Standardvärdet är falskt.|
| [language_code](/cells/sv/python-net/aspose.cells/odsloadoptions/language_code) | Hämtar eller ställer in användargränssnittsspråket för Workbook-versionen baserat på CountryCode som har sparat filen.|
| [region](/cells/sv/python-net/aspose.cells/odsloadoptions/region) | Hämtar eller ställer in systemets regionala inställningar baserat på CountryCode vid den tidpunkt då filen laddades.|
| [default_style_settings](/cells/sv/python-net/aspose.cells/odsloadoptions/default_style_settings) | Hämtar standardformatinställningarna för att initiera arbetsbokens stilar|
| [standard_font](/cells/sv/python-net/aspose.cells/odsloadoptions/standard_font) | Ställer in standardtypsnittets standardnamn|
| [standard_font_size](/cells/sv/python-net/aspose.cells/odsloadoptions/standard_font_size) | Ställer in standard standard teckenstorlek.|
| [interrupt_monitor](/cells/sv/python-net/aspose.cells/odsloadoptions/interrupt_monitor) | Hämtar och ställer in avbrottsmonitorn.|
| [ignore_not_printed](/cells/sv/python-net/aspose.cells/odsloadoptions/ignore_not_printed) | Ignorera data som inte skrivs ut om du skriver ut filen direkt|
| [check_data_valid](/cells/sv/python-net/aspose.cells/odsloadoptions/check_data_valid) |Kontrollera om data är giltiga i mallfilen.|
| [check_excel_restriction](/cells/sv/python-net/aspose.cells/odsloadoptions/check_excel_restriction) | Om kontrollera begränsning av excel-fil när användaren ändrar cellrelaterade objekt.<br/>Till exempel tillåter excel inte inmatning av strängvärden som är längre än 32K.<br/>När du matar in ett värde som är längre än 32K, till exempel Cell.PutValue(string), får du ett undantag om den här egenskapen är sann.<br/>Om den här egenskapen är falsk kommer vi att acceptera ditt inmatade strängvärde som cellens värde så att senare<br/>du kan mata ut hela strängvärdet för andra filformat som CSV.<br/>Men om du har angett en sådan typ av värde som är ogiltigt för Excel-filformat,<br/> du bör inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå ett oväntat fel för den genererade Excel-filen.|
| [keep_unparsed_data](/cells/sv/python-net/aspose.cells/odsloadoptions/keep_unparsed_data) | Behåll den oparsade datan i minnet för arbetsboken när den laddas från mallfilen. Standard är sant.|
| [load_filter](/cells/sv/python-net/aspose.cells/odsloadoptions/load_filter) | Filtret för att ange hur man laddar data.|
| [light_cells_data_handler](/cells/sv/python-net/aspose.cells/odsloadoptions/light_cells_data_handler) | Datahanteraren för att behandla celldata vid läsning av mallfil.|
| [memory_setting](/cells/sv/python-net/aspose.cells/odsloadoptions/memory_setting) | Hämtar eller ställer in alternativen för minnesanvändning.|
| [warning_callback](/cells/sv/python-net/aspose.cells/odsloadoptions/warning_callback) | Får eller ställer in varningsåteruppringning.|
| [auto_fitter_options](/cells/sv/python-net/aspose.cells/odsloadoptions/auto_fitter_options) | Hämtar och ställer in alternativen för automatisk montering|
| [auto_filter](/cells/sv/python-net/aspose.cells/odsloadoptions/auto_filter) | Indikerar om data filtreras automatiskt när filerna laddas.|
| [font_configs](/cells/sv/python-net/aspose.cells/odsloadoptions/font_configs) | Hämtar och ställer in individuella teckensnittskonfigurationer.<br/> Fungerar endast för [Workbook](/cells/sv/python-net/aspose.cells/workbook) som använder denna [LoadOptions](/cells/sv/python-net/aspose.cells/loadoptions) för att ladda.|
| [apply_excel_default_style_to_hyperlink](/cells/sv/python-net/aspose.cells/odsloadoptions/apply_excel_default_style_to_hyperlink) | Anger om standardformatet för Excel tillämpas på hyperlänk.|
| [refresh_pivot_tables](/cells/sv/python-net/aspose.cells/odsloadoptions/refresh_pivot_tables) | Anger om pivottabeller uppdateras när filen laddas.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_paper_size(type)](/cells/sv/python-net/aspose.cells/odsloadoptions/set_paper_size/#PaperSizeType) | Ställer in standardstorleken för utskriftspapper från standardskrivarens inställning.|



###  Se även
* modul [aspose.cells](..)
* klass [LoadOptions](/cells/sv/python-net/aspose.cells/loadoptions)
* klass [OdsLoadOptions](/cells/sv/python-net/aspose.cells/odsloadoptions)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
