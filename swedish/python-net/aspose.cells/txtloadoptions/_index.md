---
title: TxtLoadOptions klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1510
url: /sv/python-net/aspose.cells/txtloadoptions/
is_root: false
---
##  TxtLoadOptions klass
Representerar alternativen för att ladda textfil.



**Arv:** [TxtLoadOptions](/cells/python-net/aspose.cells/txtloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/sv/python-net/aspose.cells/loadoptions)



Typen TxtLoadOptions avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [TxtLoadOptions()](/cells/sv/python-net/aspose.cells/txtloadoptions/__init__/#) | Skapar alternativen för att ladda textfil.|
| [TxtLoadOptions(load_format)](/cells/sv/python-net/aspose.cells/txtloadoptions/__init__/#LoadFormat) | Skapar alternativen för att ladda textfil.|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [load_format](/cells/sv/python-net/aspose.cells/txtloadoptions/load_format) | Hämtar laddningsformatet.|
| [password](/cells/sv/python-net/aspose.cells/txtloadoptions/password) | Hämtar och ställer in lösenordet för arbetsboken.|
| [parsing_formula_on_open](/cells/sv/python-net/aspose.cells/txtloadoptions/parsing_formula_on_open) | Anger om formeln analyseras när filen läses.|
| [parsing_pivot_cached_records](/cells/sv/python-net/aspose.cells/txtloadoptions/parsing_pivot_cached_records) | Indikerar om tolkar pivotcachade poster när filen laddas.<br/> Standardvärdet är falskt.|
| [language_code](/cells/sv/python-net/aspose.cells/txtloadoptions/language_code) | Hämtar eller ställer in användargränssnittsspråket för Workbook-versionen baserat på CountryCode som har sparat filen.|
| [region](/cells/sv/python-net/aspose.cells/txtloadoptions/region) | Hämtar eller ställer in systemets regionala inställningar baserat på CountryCode vid den tidpunkt då filen laddades.|
| [default_style_settings](/cells/sv/python-net/aspose.cells/txtloadoptions/default_style_settings) | Hämtar standardformatinställningarna för att initiera arbetsbokens stilar|
| [standard_font](/cells/sv/python-net/aspose.cells/txtloadoptions/standard_font) | Ställer in standardtypsnittets standardnamn|
| [standard_font_size](/cells/sv/python-net/aspose.cells/txtloadoptions/standard_font_size) | Ställer in standard standard teckenstorlek.|
| [interrupt_monitor](/cells/sv/python-net/aspose.cells/txtloadoptions/interrupt_monitor) | Hämtar och ställer in avbrottsmonitorn.|
| [ignore_not_printed](/cells/sv/python-net/aspose.cells/txtloadoptions/ignore_not_printed) | Ignorera data som inte skrivs ut om du skriver ut filen direkt|
| [check_data_valid](/cells/sv/python-net/aspose.cells/txtloadoptions/check_data_valid) | Kontrollera om data är giltiga i mallfilen.|
| [check_excel_restriction](/cells/sv/python-net/aspose.cells/txtloadoptions/check_excel_restriction) | Om kontrollera begränsning av excel-fil när användaren ändrar cellrelaterade objekt.<br/>Till exempel tillåter excel inte inmatning av strängvärden som är längre än 32K.<br/>När du matar in ett värde som är längre än 32K, till exempel Cell.PutValue(string), får du ett undantag om den här egenskapen är sann.<br/>Om den här egenskapen är falsk kommer vi att acceptera ditt inmatade strängvärde som cellens värde så att senare<br/>du kan mata ut hela strängvärdet för andra filformat som CSV.<br/>Men om du har angett en sådan typ av värde som är ogiltigt för Excel-filformat,<br/> du bör inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå ett oväntat fel för den genererade Excel-filen.|
| [keep_unparsed_data](/cells/sv/python-net/aspose.cells/txtloadoptions/keep_unparsed_data) |Behåll den oparsade datan i minnet för arbetsboken när den laddas från mallfilen. Standard är sant.|
| [load_filter](/cells/sv/python-net/aspose.cells/txtloadoptions/load_filter) | Filtret för att ange hur man laddar data.|
| [light_cells_data_handler](/cells/sv/python-net/aspose.cells/txtloadoptions/light_cells_data_handler) | Datahanteraren för att behandla celldata vid läsning av mallfil.|
| [memory_setting](/cells/sv/python-net/aspose.cells/txtloadoptions/memory_setting) | Hämtar eller ställer in alternativen för minnesanvändning.|
| [warning_callback](/cells/sv/python-net/aspose.cells/txtloadoptions/warning_callback) | Får eller ställer in varningsåteruppringning.|
| [auto_fitter_options](/cells/sv/python-net/aspose.cells/txtloadoptions/auto_fitter_options) | Hämtar och ställer in alternativen för automatisk montering|
| [auto_filter](/cells/sv/python-net/aspose.cells/txtloadoptions/auto_filter) | Indikerar om data filtreras automatiskt när filerna laddas.|
| [font_configs](/cells/sv/python-net/aspose.cells/txtloadoptions/font_configs) | Hämtar och ställer in individuella teckensnittskonfigurationer.<br/> Fungerar endast för [Workbook](/cells/sv/python-net/aspose.cells/workbook) som använder denna [LoadOptions](/cells/sv/python-net/aspose.cells/loadoptions) för att ladda.|
| [encoding](/cells/sv/python-net/aspose.cells/txtloadoptions/encoding) | Hämtar och ställer in standardkodningen. Gäller endast för csv-fil.|
| [load_style_strategy](/cells/sv/python-net/aspose.cells/txtloadoptions/load_style_strategy) |Indikerar strategin för att tillämpa stil för analyserade värden vid konvertering av strängvärde till nummer eller datum och tid.|
| [convert_numeric_data](/cells/sv/python-net/aspose.cells/txtloadoptions/convert_numeric_data) | Hämtar eller ställer in ett värde som indikerar om strängen i textfilen konverteras till numerisk data.|
| [convert_date_time_data](/cells/sv/python-net/aspose.cells/txtloadoptions/convert_date_time_data) | Hämtar eller ställer in ett värde som indikerar om strängen i textfilen konverteras till datumdata.|
| [keep_precision](/cells/sv/python-net/aspose.cells/txtloadoptions/keep_precision) | Anger om ett strängvärde inte analyseras om längden är 15.|
| [separator](/cells/sv/python-net/aspose.cells/txtloadoptions/separator) |Hämtar och ställer in teckenseparator för textfil.|
| [separator_string](/cells/sv/python-net/aspose.cells/txtloadoptions/separator_string) | Hämtar och ställer in ett strängvärde som separator.|
| [is_multi_encoded](/cells/sv/python-net/aspose.cells/txtloadoptions/is_multi_encoded) | True betyder att filen innehåller flera kodningar.|
| [preferred_parsers](/cells/sv/python-net/aspose.cells/txtloadoptions/preferred_parsers) | Hämtar och ställer in föredragna värdeparsers för att ladda textfil.|
| [has_formula](/cells/sv/python-net/aspose.cells/txtloadoptions/has_formula) | Anger om texten är formel om den börjar med "=".|
| [has_text_qualifier](/cells/sv/python-net/aspose.cells/txtloadoptions/has_text_qualifier) | Om det finns textkvalificerare för cellvärde. Standard är sant.|
| [text_qualifier](/cells/sv/python-net/aspose.cells/txtloadoptions/text_qualifier) | Anger textkvalificeraren för cellvärden. Standardkvalificeraren är '''.|
| [treat_consecutive_delimiters_as_one](/cells/sv/python-net/aspose.cells/txtloadoptions/treat_consecutive_delimiters_as_one) |Huruvida konsekutiva avgränsare ska behandlas som en.|
| [treat_quote_prefix_as_value](/cells/sv/python-net/aspose.cells/txtloadoptions/treat_quote_prefix_as_value) |Anger om det inledande citattecknet ska tas som en del av värdet på en cell.<br/>Standard är sant. Om det är falskt kommer det inledande citattecken att tas bort från motsvarande cells värde<br/> och [Style.quote_prefix](/cells/sv/python-net/aspose.cells/style#quote_prefix) kommer att ställas in som sant för cellen.|
| [extend_to_next_sheet](/cells/sv/python-net/aspose.cells/txtloadoptions/extend_to_next_sheet) | Om data utökas till nästa ark när raderna eller kolumnerna med data överskrider gränsen.<br/>Om den här egenskapen är sann kommer extra data att utökas till nästa ark bakom det nuvarande (om det aktuella arket är det sista,<br/>nytt ark kommer att läggas till aktuell arbetsbok).<br/>Om den här egenskapen är falsk kommer data som överskrider gränsen att ignoreras.<br/> Standard är falskt;|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_paper_size(type)](/cells/sv/python-net/aspose.cells/txtloadoptions/set_paper_size/#PaperSizeType) | Ställer in standardstorleken för utskriftspapper från standardskrivarens inställning.|



###  Se även
* modul [aspose.cells](..)
* klass [AbstractTextLoadOptions](/cells/sv/python-net/aspose.cells/abstracttextloadoptions)
* klass [LoadOptions](/cells/sv/python-net/aspose.cells/loadoptions)
* klass [TxtLoadOptions](/cells/sv/python-net/aspose.cells/txtloadoptions)
* klass [Workbook](/cells/sv/python-net/aspose.cells/workbook)
