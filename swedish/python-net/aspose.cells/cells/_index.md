---
title: Cells klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 180
url: /sv/python-net/aspose.cells/cells/
is_root: false
---
##  Cells klass
Kapslar in en samling cellrelevanta objekt, som [Cell](/cells/sv/python-net/aspose.cells/cell), [Row](/cells/sv/python-net/aspose.cells/row), ...etc.



Typen Cells avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [ods_cell_fields](/cells/sv/python-net/aspose.cells/cells/ods_cell_fields) | Får listan över oddsfält.|
| [count](/cells/sv/python-net/aspose.cells/cells/count) | Får det totala antalet instansierade Cell objekt.|
| [count_large](/cells/sv/python-net/aspose.cells/cells/count_large) | Får det totala antalet instansierade Cell objekt.|
| [rows](/cells/sv/python-net/aspose.cells/cells/rows) | Hämtar samlingen av [Row](/cells/sv/python-net/aspose.cells/row) objekt som representerar de individuella raderna i detta kalkylblad.|
| [merged_cells](/cells/sv/python-net/aspose.cells/cells/merged_cells) | Hämtar samlingen av sammanslagna celler.|
| [multi_thread_reading](/cells/sv/python-net/aspose.cells/cells/multi_thread_reading) | Hämtar eller ställer in om celldatamodellen ska stödja multitrådsläsning.<br/> Standardvärdet för den här egenskapen är falskt.|
| [memory_setting](/cells/sv/python-net/aspose.cells/cells/memory_setting) | Hämtar eller ställer in minnesanvändningsalternativet för den här cellen.|
| [style](/cells/sv/python-net/aspose.cells/cells/style) | Hämtar och ställer in standardstilen.|
| [standard_width_inch](/cells/sv/python-net/aspose.cells/cells/standard_width_inch) |Hämtar eller ställer in standardkolumnbredden i kalkylbladet, i enheter av tum.|
| [standard_width_pixels](/cells/sv/python-net/aspose.cells/cells/standard_width_pixels) | Hämtar eller ställer in standardkolumnbredden i kalkylbladet, i enheter av pixlar.|
| [standard_width](/cells/sv/python-net/aspose.cells/cells/standard_width) | Hämtar eller ställer in standardkolumnbredden i kalkylbladet, i teckenenheter.|
| [standard_height](/cells/sv/python-net/aspose.cells/cells/standard_height) | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i poängenheter.|
| [standard_height_pixels](/cells/sv/python-net/aspose.cells/cells/standard_height_pixels) | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i enheter av pixlar.|
| [standard_height_inch](/cells/sv/python-net/aspose.cells/cells/standard_height_inch) | Hämtar eller ställer in standardradhöjden i detta kalkylblad, i enheter av tum.|
| [preserve_string](/cells/sv/python-net/aspose.cells/cells/preserve_string) | Hämtar eller ställer in ett värde som indikerar om alla kalkylbladsvärden bevaras som strängar.<br/> Standard är falskt.|
| [min_row](/cells/sv/python-net/aspose.cells/cells/min_row) | Minsta radindex för cell som innehåller data eller stil.|
| [max_row](/cells/sv/python-net/aspose.cells/cells/max_row) | Maximalt radindex för cell som innehåller data eller stil.|
| [min_column](/cells/sv/python-net/aspose.cells/cells/min_column) | Minsta kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen<br/> där stilen är definierad för hela kolumnen men ingen cell har instansierats i den).|
| [max_column](/cells/sv/python-net/aspose.cells/cells/max_column) | Minsta kolumnindex för de celler som har instansierats i samlingen (inkluderar inte kolumnen<br/> där stilen är definierad för hela kolumnen men ingen cell har instansierats i den).|
| [min_data_row](/cells/sv/python-net/aspose.cells/cells/min_data_row) | Minsta radindex för cell som innehåller data.|
| [max_data_row](/cells/sv/python-net/aspose.cells/cells/max_data_row) |Maximalt radindex för cell som innehåller data.|
| [min_data_column](/cells/sv/python-net/aspose.cells/cells/min_data_column) | Minsta kolumnindex för cell som innehåller data.|
| [max_data_column](/cells/sv/python-net/aspose.cells/cells/max_data_column) | Maximalt kolumnindex för cell som innehåller data.|
| [is_default_row_height_matched](/cells/sv/python-net/aspose.cells/cells/is_default_row_height_matched) | Indikerar att radhöjd och standardfonthöjd matchar|
| [is_default_row_hidden](/cells/sv/python-net/aspose.cells/cells/is_default_row_hidden) | Anger om raden är dold som standard.|
| [columns](/cells/sv/python-net/aspose.cells/cells/columns) | Hämtar samlingen av [Column](/cells/sv/python-net/aspose.cells/column) objekt som representerar de enskilda kolumnerna i detta kalkylblad.|
| [ranges](/cells/sv/python-net/aspose.cells/cells/ranges) | Hämtar samlingen av [Range](/cells/sv/python-net/aspose.cells/range) objekt skapade under körning.|
| [last_cell](/cells/sv/python-net/aspose.cells/cells/last_cell) | Hämtar den sista cellen i detta kalkylblad.|
| [max_display_range](/cells/sv/python-net/aspose.cells/cells/max_display_range) | Får det maximala intervallet som inkluderar data, sammanslagna celler och former.|
| [first_cell](/cells/sv/python-net/aspose.cells/cells/first_cell) | Får den första cellen i detta kalkylblad.|



Får [Cell](/cells/sv/python-net/aspose.cells/cell) objekt i kalkylbladet
###  Indexerare
| namn| Beskrivning|
| :- | :- |
| [index] | Elementets nollbaserade index.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [create_range(upper_left_cell, lower_right_cell)](/cells/sv/python-net/aspose.cells/cells/create_range/#str-str) | Skapar ett [Range](/cells/sv/python-net/aspose.cells/range)-objekt från ett cellintervall.|
| [create_range(first_row, first_column, total_rows, total_columns)](/cells/sv/python-net/aspose.cells/cells/create_range/#int-int-int-int) | Skapar ett [Range](/cells/sv/python-net/aspose.cells/range)-objekt från ett cellintervall.|
| [create_range(address)](/cells/sv/python-net/aspose.cells/cells/create_range/#str) | Skapar ett [Range](/cells/sv/python-net/aspose.cells/range)-objekt från en adress i intervallet.|
| [create_range(first_index, number, is_vertical)](/cells/sv/python-net/aspose.cells/cells/create_range/#int-int-bool) | Skapar ett [Range](/cells/sv/python-net/aspose.cells/range)-objekt från rader med celler eller kolumner med celler.|
| [get(row, column)](/cells/sv/python-net/aspose.cells/cells/get/#int-int) |Lägg till API for Python Via .Net.eftersom denna [int rad, int kolumn] inte stöds|
| [get(cell_name)](/cells/sv/python-net/aspose.cells/cells/get/#str) | Lägg till API for Python Via .Net.eftersom denna [sträng cellnamn] inte stöds|
| [import_object_array(obj_array, first_row, first_column, is_vertical)](/cells/sv/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool) | Importerar en mängd data till ett kalkylblad.|
| [import_object_array(obj_array, first_row, first_column, is_vertical, skip)](/cells/sv/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool-int) | Importerar en mängd data till ett kalkylblad.|
| [import_array(string_array, first_row, first_column, is_vertical)](/cells/sv/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importerar en uppsättning strängar till ett kalkylblad.|
| [import_array(int_array, first_row, first_column, is_vertical)](/cells/sv/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importerar en matris med heltal till ett kalkylblad.|
| [import_array(double_array, first_row, first_column, is_vertical)](/cells/sv/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importerar en array av dubblar till ett kalkylblad.|
| [import_csv(file_name, splitter, convert_numeric_data, first_row, first_column)](/cells/sv/python-net/aspose.cells/cells/import_csv/#str-str-bool-int-int) | Importera en CSV-fil till cellerna.|
| [import_csv(stream, splitter, convert_numeric_data, first_row, first_column)](/cells/sv/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-str-bool-int-int) | Importera en CSV-fil till cellerna.|
| [import_csv(file_name, options, first_row, first_column)](/cells/sv/python-net/aspose.cells/cells/import_csv/#str-TxtLoadOptions-int-int) | Importera en CSV-fil till cellerna.|
| [import_csv(stream, options, first_row, first_column)](/cells/sv/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-TxtLoadOptions-int-int) | Importera en CSV-fil till cellerna.|
| [merge(first_row, first_column, total_rows, total_columns)](/cells/sv/python-net/aspose.cells/cells/merge/#int-int-int-int) | Slår samman ett specificerat cellområde till en enda cell.|
| [merge(first_row, first_column, total_rows, total_columns, merge_conflict)](/cells/sv/python-net/aspose.cells/cells/merge/#int-int-int-int-bool) | Slår samman ett specificerat cellområde till en enda cell.|
| [merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict)](/cells/sv/python-net/aspose.cells/cells/merge/#int-int-int-int-bool-bool) | Slår samman ett specificerat cellområde till en enda cell.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number, paste_options)](/cells/sv/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-PasteOptions) | Kopierar data och format för en hel kolumn.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number)](/cells/sv/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int) | Kopierar data och format för en hel kolumn.|
| [copy_columns(source_cells, source_column_index, source_total_columns, destination_column_index, destination_total_columns)](/cells/sv/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-int) | Kopierar data och format för hela kolumnerna.|
| [copy_rows(source_cells, source_row_index, destination_row_index, row_number)](/cells/sv/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int) | Kopierar data och format för vissa hela rader.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options)](/cells/sv/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions) | Kopierar data och format för vissa hela rader.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options, paste_options)](/cells/sv/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions-PasteOptions) | Kopierar data och format för vissa hela rader.|
| [group_columns(first_index, last_index)](/cells/sv/python-net/aspose.cells/cells/group_columns/#int-int) | Gruppera kolumner.|
| [group_columns(first_index, last_index, is_hidden)](/cells/sv/python-net/aspose.cells/cells/group_columns/#int-int-bool) | Gruppera kolumner.|
| [ungroup_rows(first_index, last_index, is_all)](/cells/sv/python-net/aspose.cells/cells/ungroup_rows/#int-int-bool) | Dela upp rader.|
| [ungroup_rows(first_index, last_index)](/cells/sv/python-net/aspose.cells/cells/ungroup_rows/#int-int) | Dela upp rader.|
| [group_rows(first_index, last_index, is_hidden)](/cells/sv/python-net/aspose.cells/cells/group_rows/#int-int-bool) | Grupperar rader.|
| [group_rows(first_index, last_index)](/cells/sv/python-net/aspose.cells/cells/group_rows/#int-int) | Grupperar rader.|
| [delete_column(column_index, update_reference)](/cells/sv/python-net/aspose.cells/cells/delete_column/#int-bool) | Tar bort en kolumn.|
| [delete_column(column_index)](/cells/sv/python-net/aspose.cells/cells/delete_column/#int) | Tar bort en kolumn.|
| [delete_rows(row_index, total_rows)](/cells/sv/python-net/aspose.cells/cells/delete_rows/#int-int) | Tar bort flera rader.|
| [delete_rows(row_index, total_rows, update_reference)](/cells/sv/python-net/aspose.cells/cells/delete_rows/#int-int-bool) | Tar bort flera rader i kalkylbladet.|
| [delete_blank_columns()](/cells/sv/python-net/aspose.cells/cells/delete_blank_columns/#) | Ta bort alla tomma kolumner som inte innehåller några data.|
| [delete_blank_columns(options)](/cells/sv/python-net/aspose.cells/cells/delete_blank_columns/#DeleteOptions) | Ta bort alla tomma kolumner som inte innehåller några data.|
| [delete_blank_rows()](/cells/sv/python-net/aspose.cells/cells/delete_blank_rows/#) | Ta bort alla tomma rader som inte innehåller några data.|
| [delete_blank_rows(options)](/cells/sv/python-net/aspose.cells/cells/delete_blank_rows/#DeleteOptions) | Ta bort alla tomma rader som inte innehåller några data.|
| [insert_columns(column_index, total_columns)](/cells/sv/python-net/aspose.cells/cells/insert_columns/#int-int) | Infogar några kolumner i kalkylbladet.|
| [insert_columns(column_index, total_columns, update_reference)](/cells/sv/python-net/aspose.cells/cells/insert_columns/#int-int-bool) | Infogar några kolumner i kalkylbladet.|
| [insert_column(column_index, update_reference)](/cells/sv/python-net/aspose.cells/cells/insert_column/#int-bool) |Infogar en ny kolumn i kalkylbladet.|
| [insert_column(column_index)](/cells/sv/python-net/aspose.cells/cells/insert_column/#int) |Infogar en ny kolumn i kalkylbladet.|
| [insert_rows(row_index, total_rows, update_reference)](/cells/sv/python-net/aspose.cells/cells/insert_rows/#int-int-bool) | Infogar flera rader i kalkylbladet.|
| [insert_rows(row_index, total_rows, options)](/cells/sv/python-net/aspose.cells/cells/insert_rows/#int-int-InsertOptions) | Infogar flera rader i kalkylbladet.|
| [insert_rows(row_index, total_rows)](/cells/sv/python-net/aspose.cells/cells/insert_rows/#int-int) | Infogar flera rader i kalkylbladet.|
| [clear_range(range)](/cells/sv/python-net/aspose.cells/cells/clear_range/#CellArea) | Rensar innehåll och formatering av ett intervall.|
| [clear_range(start_row, start_column, end_row, end_column)](/cells/sv/python-net/aspose.cells/cells/clear_range/#int-int-int-int) | Rensar innehåll och formatering av ett intervall.|
| [clear_contents(range)](/cells/sv/python-net/aspose.cells/cells/clear_contents/#CellArea) | Rensar innehållet i ett intervall.|
| [clear_contents(start_row, start_column, end_row, end_column)](/cells/sv/python-net/aspose.cells/cells/clear_contents/#int-int-int-int) | Rensar innehållet i ett intervall.|
| [clear_formats(range)](/cells/sv/python-net/aspose.cells/cells/clear_formats/#CellArea) | Rensar formatering av ett intervall.|
| [clear_formats(start_row, start_column, end_row, end_column)](/cells/sv/python-net/aspose.cells/cells/clear_formats/#int-int-int-int) | Rensar formatering av ett intervall.|
| [find(what, previous_cell)](/cells/sv/python-net/aspose.cells/cells/find/#any-Cell) | Hittar cellen som innehåller inmatningsobjektet.|
| [find(what, previous_cell, find_options)](/cells/sv/python-net/aspose.cells/cells/find/#any-Cell-FindOptions) | Hittar cellen som innehåller inmatningsobjektet.|
| [end_cell_in_row(row_index)](/cells/sv/python-net/aspose.cells/cells/end_cell_in_row/#int) | Får den sista cellen i den här raden.|
| [end_cell_in_row(start_row, end_row, start_column, end_column)](/cells/sv/python-net/aspose.cells/cells/end_cell_in_row/#int-int-int-int) | Hämtar den sista cellen med maximalt radindex i detta intervall.|
| [end_cell_in_column(column_index)](/cells/sv/python-net/aspose.cells/cells/end_cell_in_column/#int) | Hämtar den sista cellen i denna kolumn.|
| [end_cell_in_column(start_row, end_row, start_column, end_column)](/cells/sv/python-net/aspose.cells/cells/end_cell_in_column/#int-int-int-int) | Hämtar den sista cellen med maximalt kolumnindex i detta intervall.|
| [insert_range(area, shift_number, shift_type, update_reference)](/cells/sv/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType-bool) | Infogar ett intervall av celler och skift celler enligt skiftalternativet.|
| [insert_range(area, shift_type)](/cells/sv/python-net/aspose.cells/cells/insert_range/#CellArea-ShiftType) | Infogar ett intervall av celler och skift celler enligt skiftalternativet.|
| [insert_range(area, shift_number, shift_type)](/cells/sv/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType) | Infogar ett intervall av celler och skift celler enligt skiftalternativet.|
| [import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number)](/cells/sv/python-net/aspose.cells/cells/import_custom_objects/#list-list-bool-int-int-int-bool-str-bool) | Importerar anpassade objekt.|
| [import_custom_objects(list, first_row, first_column, options)](/cells/sv/python-net/aspose.cells/cells/import_custom_objects/#list-int-int-ImportTableOptions) | Importerar anpassade objekt.|
| [subtotal(ca, group_by, function, total_list)](/cells/sv/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list) | Skapar delsummor för intervallet.|
| [subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data)](/cells/sv/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list-bool-bool-bool) | Skapar delsummor för intervallet.|
| [remove_duplicates()](/cells/sv/python-net/aspose.cells/cells/remove_duplicates/#) | Tar bort dubbletter av rader i arket.|
| [remove_duplicates(start_row, start_column, end_row, end_column)](/cells/sv/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int) | Tar bort dubbletter av värden i intervallet.|
| [remove_duplicates(start_row, start_column, end_row, end_column, has_headers, column_offsets)](/cells/sv/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int-bool-list) | Tar bort dubbletter av data från intervallet.|
| [get_row_enumerator()](/cells/sv/python-net/aspose.cells/cells/get_row_enumerator/#) | Hämtar raduppräkningen.|
| [get_cell(row, column)](/cells/sv/python-net/aspose.cells/cells/get_cell/#int-int) | Hämtar elementet [Cell](/cells/sv/python-net/aspose.cells/cell) eller null vid angivet cellradindex och kolumnindex.|
| [get_row(row)](/cells/sv/python-net/aspose.cells/cells/get_row/#int) | Hämtar elementet [Row](/cells/sv/python-net/aspose.cells/row) vid angivet cellradsindex.|
| [check_cell(row, column)](/cells/sv/python-net/aspose.cells/cells/check_cell/#int-int) | Hämtar elementet [Cell](/cells/sv/python-net/aspose.cells/cell) eller null vid angivet cellradindex och kolumnindex.|
| [check_row(row)](/cells/sv/python-net/aspose.cells/cells/check_row/#int) |Hämtar elementet [Row](/cells/sv/python-net/aspose.cells/row) eller vid angivet cellradsindex.|
| [check_column(column_index)](/cells/sv/python-net/aspose.cells/cells/check_column/#int) | Hämtar elementet [Column](/cells/sv/python-net/aspose.cells/column) eller null vid det angivna kolumnindexet.|
| [is_row_hidden(row_index)](/cells/sv/python-net/aspose.cells/cells/is_row_hidden/#int) | Kontrollerar om en rad vid ett givet index är dold.|
| [is_column_hidden(column_index)](/cells/sv/python-net/aspose.cells/cells/is_column_hidden/#int) | Kontrollerar om en kolumn vid ett givet index är dold.|
| [add_range(range_object)](/cells/sv/python-net/aspose.cells/cells/add_range/#Range) | Lägger till en intervallobjektreferens till celler|
| [clear()](/cells/sv/python-net/aspose.cells/cells/clear/#) | Rensar alla cell- och radobjekt.|
| [import_data(table, first_row, first_column, options)](/cells/sv/python-net/aspose.cells/cells/import_data/#ICellsDataTable-int-int-ImportTableOptions) | Importera data från anpassad datatabell.|
| [import_array_list(array_list, first_row, first_column, is_vertical)](/cells/sv/python-net/aspose.cells/cells/import_array_list/#list-int-int-bool) | Importerar en arraylista med data till ett kalkylblad.|
| [import_formula_array(string_array, first_row, first_column, is_vertical)](/cells/sv/python-net/aspose.cells/cells/import_formula_array/#list-int-int-bool) | Importerar en matris med formler till ett kalkylblad.|
| [text_to_columns(row, column, total_rows, options)](/cells/sv/python-net/aspose.cells/cells/text_to_columns/#int-int-int-TxtLoadOptions) | Delar upp texten i kolumnerna till kolumner.|
| [un_merge(first_row, first_column, total_rows, total_columns)](/cells/sv/python-net/aspose.cells/cells/un_merge/#int-int-int-int) | Tar bort ett specificerat intervall av sammanslagna celler.|
| [clear_merged_cells()](/cells/sv/python-net/aspose.cells/cells/clear_merged_cells/#) | Rensar alla sammanslagna intervall.|
| [hide_row(row)](/cells/sv/python-net/aspose.cells/cells/hide_row/#int) | Döljer en rad.|
| [unhide_row(row, height)](/cells/sv/python-net/aspose.cells/cells/unhide_row/#int-float) | Visa en rad.|
| [hide_rows(row, total_rows)](/cells/sv/python-net/aspose.cells/cells/hide_rows/#int-int) | Döljer flera rader.|
| [unhide_rows(row, total_rows, height)](/cells/sv/python-net/aspose.cells/cells/unhide_rows/#int-int-float) | Visar de dolda raderna.|
| [set_row_height_pixel(row, pixels)](/cells/sv/python-net/aspose.cells/cells/set_row_height_pixel/#int-int) | Ställer in radhöjden i pixelenhet.|
| [set_row_height_inch(row, inches)](/cells/sv/python-net/aspose.cells/cells/set_row_height_inch/#int-float) | Ställer in radhöjden i enheter av tum.|
| [set_row_height(row, height)](/cells/sv/python-net/aspose.cells/cells/set_row_height/#int-float) | Ställer in höjden på den angivna raden.|
| [get_row_original_height_point(row)](/cells/sv/python-net/aspose.cells/cells/get_row_original_height_point/#int) | Får den ursprungliga radens höjd i punktenhet om raden är dold|
| [hide_column(column)](/cells/sv/python-net/aspose.cells/cells/hide_column/#int) | Döljer en kolumn.|
| [unhide_column(column, width)](/cells/sv/python-net/aspose.cells/cells/unhide_column/#int-float) | Visa en kolumn|
| [hide_columns(column, total_columns)](/cells/sv/python-net/aspose.cells/cells/hide_columns/#int-int) | Dölj flera kolumner.|
| [unhide_columns(column, total_columns, width)](/cells/sv/python-net/aspose.cells/cells/unhide_columns/#int-int-float) |Visa flera kolumner.|
| [get_row_height(row)](/cells/sv/python-net/aspose.cells/cells/get_row_height/#int) | Hämtar höjden på en angiven rad.|
| [get_view_row_height(row)](/cells/sv/python-net/aspose.cells/cells/get_view_row_height/#int) | Hämtar höjden på en angiven rad.|
| [get_row_height_pixel(row)](/cells/sv/python-net/aspose.cells/cells/get_row_height_pixel/#int) | Hämtar höjden på en angiven rad i pixelenhet.|
| [get_row_height_inch(row)](/cells/sv/python-net/aspose.cells/cells/get_row_height_inch/#int) | Hämtar höjden på en angiven rad i enheter av tum.|
| [get_view_row_height_inch(row)](/cells/sv/python-net/aspose.cells/cells/get_view_row_height_inch/#int) | Hämtar höjden på en angiven rad i enheter av tum.|
| [set_column_width_pixel(column, pixels)](/cells/sv/python-net/aspose.cells/cells/set_column_width_pixel/#int-int) | Ställer in kolumnbredden i pixelenhet i normal vy.|
| [set_column_width_inch(column, inches)](/cells/sv/python-net/aspose.cells/cells/set_column_width_inch/#int-float) | Ställer in kolumnbredden i tumenhet i normalvy.|
| [set_column_width(column, width)](/cells/sv/python-net/aspose.cells/cells/set_column_width/#int-float) | Ställer in bredden på den angivna kolumnen i normal vy.|
| [get_column_width_pixel(column)](/cells/sv/python-net/aspose.cells/cells/get_column_width_pixel/#int) | Hämtar bredden på den angivna kolumnen i normal vy, i enheter av pixlar.|
| [get_column_width_inch(column)](/cells/sv/python-net/aspose.cells/cells/get_column_width_inch/#int) | Hämtar bredden på den angivna kolumnen i normalvy, i enheter av tum.|
| [get_column_width(column)](/cells/sv/python-net/aspose.cells/cells/get_column_width/#int) | Hämtar bredden på den angivna kolumnen i normal vy|
| [get_view_column_width_pixel(column)](/cells/sv/python-net/aspose.cells/cells/get_view_column_width_pixel/#int) | Få bredden i olika vytyper.|
| [set_view_column_width_pixel(column, pixels)](/cells/sv/python-net/aspose.cells/cells/set_view_column_width_pixel/#int-int) | Ställer in bredden på kolumnen i olika vyer.|
| [get_last_data_row(column)](/cells/sv/python-net/aspose.cells/cells/get_last_data_row/#int) | Hämtar den sista radens index i cellen som innehåller data i den angivna kolumnen.|
| [apply_column_style(column, style, flag)](/cells/sv/python-net/aspose.cells/cells/apply_column_style/#int-Style-StyleFlag) | Tillämpar format för en hel kolumn.|
| [apply_row_style(row, style, flag)](/cells/sv/python-net/aspose.cells/cells/apply_row_style/#int-Style-StyleFlag) | Använder format för en hel rad.|
| [apply_style(style, flag)](/cells/sv/python-net/aspose.cells/cells/apply_style/#Style-StyleFlag) | Tillämpar format för ett helt kalkylblad.|
| [copy_column(source_cells, source_column_index, destination_column_index)](/cells/sv/python-net/aspose.cells/cells/copy_column/#Cells-int-int) | Kopierar data och format för en hel kolumn.|
| [copy_row(source_cells, source_row_index, destination_row_index)](/cells/sv/python-net/aspose.cells/cells/copy_row/#Cells-int-int) | Kopierar data och format för en hel rad.|
| [get_grouped_row_outline_level(row_index)](/cells/sv/python-net/aspose.cells/cells/get_grouped_row_outline_level/#int) |Hämtar konturnivån (nollbaserad) för raden.|
| [get_grouped_column_outline_level(column_index)](/cells/sv/python-net/aspose.cells/cells/get_grouped_column_outline_level/#int) | Hämtar konturnivån (nollbaserad) för kolumnen.|
| [get_max_grouped_column_outline_level()](/cells/sv/python-net/aspose.cells/cells/get_max_grouped_column_outline_level/#) | Hämtar den maximala grupperade kolumnkonturnivån (nollbaserad).|
| [get_max_grouped_row_outline_level()](/cells/sv/python-net/aspose.cells/cells/get_max_grouped_row_outline_level/#) | Får den maximala grupperade radkonturnivån (nollbaserad).|
| [show_group_detail(is_vertical, index)](/cells/sv/python-net/aspose.cells/cells/show_group_detail/#bool-int) | Expanderar de grupperade raderna/kolumnerna.|
| [hide_group_detail(is_vertical, index)](/cells/sv/python-net/aspose.cells/cells/hide_group_detail/#bool-int) | Komprimerar de grupperade raderna/kolumnerna.|
| [ungroup_columns(first_index, last_index)](/cells/sv/python-net/aspose.cells/cells/ungroup_columns/#int-int) | Delar upp kolumner.|
| [delete_columns(column_index, total_columns, update_reference)](/cells/sv/python-net/aspose.cells/cells/delete_columns/#int-int-bool) | Tar bort flera kolumner.|
| [is_deleting_range_enabled(start_row, start_column, total_rows, total_columns)](/cells/sv/python-net/aspose.cells/cells/is_deleting_range_enabled/#int-int-int-int) | Kontrollera om intervallet kan raderas.|
| [delete_row(row_index)](/cells/sv/python-net/aspose.cells/cells/delete_row/#int) | Tar bort en rad.|
| [is_blank_column(column_index)](/cells/sv/python-net/aspose.cells/cells/is_blank_column/#int) | Kontrollerar om given kolumn är tom (innehåller inga data).|
| [insert_row(row_index)](/cells/sv/python-net/aspose.cells/cells/insert_row/#int) | Infogar en ny rad i kalkylbladet.|
| [link_to_xml_map(map_name, row, column, path)](/cells/sv/python-net/aspose.cells/cells/link_to_xml_map/#str-int-int-str) | Länk till en xml-karta.|
| [find_formula(formula, previous_cell)](/cells/sv/python-net/aspose.cells/cells/find_formula/#str-Cell) | Hittar cellen med inmatningssträngen.|
| [find_formula_contains(formula, previous_cell)](/cells/sv/python-net/aspose.cells/cells/find_formula_contains/#str-Cell) | Hittar cellen med formeln som innehåller inmatningssträngen.|
| [move_range(source_area, dest_row, dest_column)](/cells/sv/python-net/aspose.cells/cells/move_range/#CellArea-int-int) | Flyttar intervallet.|
| [insert_cut_cells(cut_range, row, column, shift_type)](/cells/sv/python-net/aspose.cells/cells/insert_cut_cells/#Range-int-int-ShiftType) | Skärområde för insättning.|
| [delete_range(start_row, start_column, end_row, end_column, shift_type)](/cells/sv/python-net/aspose.cells/cells/delete_range/#int-int-int-int-ShiftType) | Tar bort ett intervall av celler och skiftar celler enligt skiftalternativet.|
| [retrieve_subtotal_setting(ca)](/cells/sv/python-net/aspose.cells/cells/retrieve_subtotal_setting/#CellArea) | Hämtar inställning av delsummor för intervallet.|
| [remove_formulas()](/cells/sv/python-net/aspose.cells/cells/remove_formulas/#) | Tar bort alla formler och ersätter med formelns värde.|
| [convert_string_to_numeric_value()](/cells/sv/python-net/aspose.cells/cells/convert_string_to_numeric_value/#) |Konverterar strängdata i celler till numeriska värden om möjligt.|
| [get_dependents(is_all, row, column)](/cells/sv/python-net/aspose.cells/cells/get_dependents/#bool-int-int) | Få alla celler som refererar till den specifika cellen.|
| [get_dependents_in_calculation(row, column, recursive)](/cells/sv/python-net/aspose.cells/cells/get_dependents_in_calculation/#int-int-bool) | Hämtar alla celler vars beräknade resultat beror på specifika celler.|
| [get_cell_style(row, column)](/cells/sv/python-net/aspose.cells/cells/get_cell_style/#int-int) | Få stilen för given cell.|



###  Se även
* modul [aspose.cells](..)
* klass [Cell](/cells/sv/python-net/aspose.cells/cell)
* klass [Column](/cells/sv/python-net/aspose.cells/column)
* klass [Range](/cells/sv/python-net/aspose.cells/range)
* klass [Row](/cells/sv/python-net/aspose.cells/row)
