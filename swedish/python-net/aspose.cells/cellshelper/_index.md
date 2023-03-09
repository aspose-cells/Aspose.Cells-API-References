---
title: CellsHelper klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 230
url: /sv/python-net/aspose.cells/cellshelper/
is_root: false
---
##  CellsHelper klass
Tillhandahåller hjälpfunktioner.



Typen CellsHelper avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [significant_digits](/cells/sv/python-net/aspose.cells/cellshelper/significant_digits) | Hämtar och ställer in antalet signifikanta siffror.<br/> Standardvärdet är 17.|
| [dpi](/cells/sv/python-net/aspose.cells/cellshelper/dpi) | Får maskinens DPI.|
| [startup_path](/cells/sv/python-net/aspose.cells/cellshelper/startup_path) |Hämtar eller ställer in startsökvägen, som refereras till av vissa externa formelreferenser.|
| [alt_start_path](/cells/sv/python-net/aspose.cells/cellshelper/alt_start_path) | Hämtar eller ställer in den alternativa startsökvägen, som refereras till av vissa externa formelreferenser.|
| [library_path](/cells/sv/python-net/aspose.cells/cellshelper/library_path) | Hämtar eller ställer in bibliotekssökvägen som hänvisas till av vissa externa formelreferenser.|
| [custom_implementation_factory](/cells/sv/python-net/aspose.cells/cellshelper/custom_implementation_factory) | Får eller ställer in fabriken för att skapa instanser med speciell implementering.|
| [is_cloud_platform](/cells/sv/python-net/aspose.cells/cellshelper/is_cloud_platform) | Vänligen ange den här egenskapen True när du kör på en molnplattform, som: Azure, AWSLambda, etc,|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [create_safe_sheet_name(name_proposal)](/cells/sv/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str) | Kontrollerar det angivna arknamnet och skapar ett giltigt vid behov.<br/>Om det angivna arknamnet överensstämmer med reglerna för Excel-arknamn, returnera det.<br/>Annars kommer strängen att trunkeras om längden överskrider gränsen<br/> och ogiltiga tecken kommer att ersättas med ' ', och returnerar sedan det ombyggda strängvärdet.|
| [create_safe_sheet_name(name_proposal, replace_char)](/cells/sv/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str-char) | Kontrollerar det angivna arknamnet och skapar ett giltigt vid behov.<br/>Om det angivna arknamnet överensstämmer med reglerna för Excel-arknamn, returnera det.<br/>Annars kommer strängen att trunkeras om längden överskrider gränsen<br/> och ogiltiga tecken kommer att ersättas med ett givet tecken, och returnerar sedan det ombyggda strängvärdet.|
| [get_text_width(text, font, scaling)](/cells/sv/python-net/aspose.cells/cellshelper/get_text_width/#str-Font-float) | Få textens bredd i poängenhet.|
| [get_version()](/cells/sv/python-net/aspose.cells/cellshelper/get_version/#) | Hämta releaseversionen.|
| [cell_name_to_index(cell_name, row, column)](/cells/sv/python-net/aspose.cells/cellshelper/cell_name_to_index/#str-any-any) | Hämtar cellrads- och kolumnindex enligt dess namn.|
| [cell_index_to_name(row, column)](/cells/sv/python-net/aspose.cells/cellshelper/cell_index_to_name/#int-int) | Hämtar cellnamn enligt dess rad- och kolumnindex.|
| [column_index_to_name(column)](/cells/sv/python-net/aspose.cells/cellshelper/column_index_to_name/#int) | Hämtar kolumnnamn enligt kolumnindex.|
| [column_name_to_index(column_name)](/cells/sv/python-net/aspose.cells/cellshelper/column_name_to_index/#str) |Hämtar kolumnindex enligt kolumnnamn.|
| [row_index_to_name(row)](/cells/sv/python-net/aspose.cells/cellshelper/row_index_to_name/#int) | Hämtar radnamn enligt radindex.|
| [row_name_to_index(row_name)](/cells/sv/python-net/aspose.cells/cellshelper/row_name_to_index/#str) | Får radindex enligt radnamn.|
| [convert_r1c1_formula_to_a1(r_1c1_formula, row, column)](/cells/sv/python-net/aspose.cells/cellshelper/convert_r1c1_formula_to_a1/#str-int-int) | Konverterar cellens r1c1-formel till A1-formeln.|
| [convert_a1_formula_to_r1c1(formula, row, column)](/cells/sv/python-net/aspose.cells/cellshelper/convert_a1_formula_to_r1c1/#str-int-int) | Konverterar A1-formeln för cellen till r1c1-formeln.|
| [get_date_time_from_double(double_value, date1904)](/cells/sv/python-net/aspose.cells/cellshelper/get_date_time_from_double/#float-bool) | Konvertera det dubbla värdet till datum och tid.|
| [get_double_from_date_time(date_time, date1904)](/cells/sv/python-net/aspose.cells/cellshelper/get_double_from_date_time/#DateTime-bool) | Konvertera datum och tid till dubbelt värde.|
| [get_used_colors(workbook)](/cells/sv/python-net/aspose.cells/cellshelper/get_used_colors/#Workbook) | Får alla använda färger i arbetsboken.|
| [add_add_in_function(function, min_count_of_parameters, max_count_of_parameters, paramers_type, function_value_type)](/cells/sv/python-net/aspose.cells/cellshelper/add_add_in_function/#str-int-int-list-ParameterType) | Lägg till tilläggsfunktion.|
| [merge_files(files, cached_file, dest_file)](/cells/sv/python-net/aspose.cells/cellshelper/merge_files/#list-str-str) | Slår ihop några stora xls-filer till en xls-fil.|
| [init_for_dot_net_core()](/cells/sv/python-net/aspose.cells/cellshelper/init_for_dot_net_core/#) | Gör initieringen för .NetCore-programmet.<br/> Vi föreslår att du först anropar den här metoden för all .NetCore-initiering.<br/>Till exempel:<br/>CellsHelper.InitForDotNetCore();<br/> Arbetsbok wb = ny arbetsbok();|



###  Se även
* modul [aspose.cells](..)
