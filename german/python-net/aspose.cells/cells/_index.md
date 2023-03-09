---
title: Cells Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 180
url: /de/python-net/aspose.cells/cells/
is_root: false
---
##  Cells Klasse
Kapselt eine Sammlung von zellrelevanten Objekten, wie z. B. [Cell](/cells/de/python-net/aspose.cells/cell), [Row](/cells/de/python-net/aspose.cells/row) usw.



Der Typ Cells macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [ods_cell_fields](/cells/de/python-net/aspose.cells/cells/ods_cell_fields) | Ruft die Liste der Quotenfelder ab.|
| [count](/cells/de/python-net/aspose.cells/cells/count) | Ruft die Gesamtzahl der instanziierten Cell-Objekte ab.|
| [count_large](/cells/de/python-net/aspose.cells/cells/count_large) | Ruft die Gesamtzahl der instanziierten Cell-Objekte ab.|
| [rows](/cells/de/python-net/aspose.cells/cells/rows) | Ruft die Auflistung von [Row](/cells/de/python-net/aspose.cells/row)-Objekten ab, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen.|
| [merged_cells](/cells/de/python-net/aspose.cells/cells/merged_cells) | Ruft die Auflistung verbundener Zellen ab.|
| [multi_thread_reading](/cells/de/python-net/aspose.cells/cells/multi_thread_reading) | Ruft ab oder legt fest, ob das Zellendatenmodell Multi-Thread-Lesen unterstützen soll.<br/> Der Standardwert dieser Eigenschaft ist false.|
| [memory_setting](/cells/de/python-net/aspose.cells/cells/memory_setting) | Ruft die Speichernutzungsoption für diese Zelle ab oder legt diese fest.|
| [style](/cells/de/python-net/aspose.cells/cells/style) | Ruft den Standardstil ab und legt ihn fest.|
| [standard_width_inch](/cells/de/python-net/aspose.cells/cells/standard_width_inch) |Ruft die Standardspaltenbreite im Arbeitsblatt in Zolleinheiten ab oder legt diese fest.|
| [standard_width_pixels](/cells/de/python-net/aspose.cells/cells/standard_width_pixels) | Ruft die Standardspaltenbreite im Arbeitsblatt in Pixeleinheiten ab oder legt diese fest.|
| [standard_width](/cells/de/python-net/aspose.cells/cells/standard_width) | Ruft die Standardspaltenbreite im Arbeitsblatt in Zeicheneinheiten ab oder legt diese fest.|
| [standard_height](/cells/de/python-net/aspose.cells/cells/standard_height) | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Punkteinheiten ab oder legt diese fest.|
| [standard_height_pixels](/cells/de/python-net/aspose.cells/cells/standard_height_pixels) | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Pixeleinheiten ab oder legt diese fest.|
| [standard_height_inch](/cells/de/python-net/aspose.cells/cells/standard_height_inch) | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Zolleinheiten ab oder legt diese fest.|
| [preserve_string](/cells/de/python-net/aspose.cells/cells/preserve_string) | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob alle Arbeitsblattwerte als Zeichenfolgen beibehalten werden.<br/> Standard ist falsch.|
| [min_row](/cells/de/python-net/aspose.cells/cells/min_row) | Minimaler Zeilenindex der Zelle, die Daten oder Stil enthält.|
| [max_row](/cells/de/python-net/aspose.cells/cells/max_row) | Maximaler Zeilenindex der Zelle, die Daten oder Stil enthält.|
| [min_column](/cells/de/python-net/aspose.cells/cells/min_column) | Minimaler Spaltenindex der Zellen, die in der Sammlung instanziiert wurden (enthält nicht die Spalte<br/> wobei der Stil für die gesamte Spalte definiert ist, aber keine Zelle darin instanziiert wurde).|
| [max_column](/cells/de/python-net/aspose.cells/cells/max_column) | Minimaler Spaltenindex der Zellen, die in der Sammlung instanziiert wurden (enthält nicht die Spalte<br/> wobei der Stil für die gesamte Spalte definiert ist, aber keine Zelle darin instanziiert wurde).|
| [min_data_row](/cells/de/python-net/aspose.cells/cells/min_data_row) | Minimaler Zeilenindex der Zelle, die Daten enthält.|
| [max_data_row](/cells/de/python-net/aspose.cells/cells/max_data_row) |Maximaler Zeilenindex der Zelle, die Daten enthält.|
| [min_data_column](/cells/de/python-net/aspose.cells/cells/min_data_column) | Minimaler Spaltenindex der Zelle, die Daten enthält.|
| [max_data_column](/cells/de/python-net/aspose.cells/cells/max_data_column) | Maximaler Spaltenindex der Zelle, die Daten enthält.|
| [is_default_row_height_matched](/cells/de/python-net/aspose.cells/cells/is_default_row_height_matched) | Gibt an, dass die Zeilenhöhe und die Standardschrifthöhe übereinstimmen|
| [is_default_row_hidden](/cells/de/python-net/aspose.cells/cells/is_default_row_hidden) | Gibt an, ob die Zeile standardmäßig ausgeblendet ist.|
| [columns](/cells/de/python-net/aspose.cells/cells/columns) | Ruft die Auflistung von [Column](/cells/de/python-net/aspose.cells/column)-Objekten ab, die die einzelnen Spalten in diesem Arbeitsblatt darstellen.|
| [ranges](/cells/de/python-net/aspose.cells/cells/ranges) | Ruft die Sammlung von [Range](/cells/de/python-net/aspose.cells/range)-Objekten ab, die zur Laufzeit erstellt wurden.|
| [last_cell](/cells/de/python-net/aspose.cells/cells/last_cell) | Ruft die letzte Zelle in diesem Arbeitsblatt ab.|
| [max_display_range](/cells/de/python-net/aspose.cells/cells/max_display_range) | Ruft den maximalen Bereich ab, der Daten, verbundene Zellen und Formen umfasst.|
| [first_cell](/cells/de/python-net/aspose.cells/cells/first_cell) | Ruft die erste Zelle in diesem Arbeitsblatt ab.|



Ruft [Cell](/cells/de/python-net/aspose.cells/cell)-Element im Arbeitsblatt ab
###  Indexierer
| Name| Beschreibung|
| :- | :- |
| [index] | Der nullbasierte Index des Elements.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [create_range(upper_left_cell, lower_right_cell)](/cells/de/python-net/aspose.cells/cells/create_range/#str-str) | Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus einem Zellbereich.|
| [create_range(first_row, first_column, total_rows, total_columns)](/cells/de/python-net/aspose.cells/cells/create_range/#int-int-int-int) | Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus einem Zellbereich.|
| [create_range(address)](/cells/de/python-net/aspose.cells/cells/create_range/#str) | Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus einer Adresse des Bereichs.|
| [create_range(first_index, number, is_vertical)](/cells/de/python-net/aspose.cells/cells/create_range/#int-int-bool) | Erstellt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt aus Zeilen von Zellen oder Spalten von Zellen.|
| [get(row, column)](/cells/de/python-net/aspose.cells/cells/get/#int-int) |Fügen Sie API for Python über .Net hinzu, da dies [int-Zeile, int-Spalte] nicht unterstützt wird|
| [get(cell_name)](/cells/de/python-net/aspose.cells/cells/get/#str) | Fügen Sie API for Python über .Net hinzu, da diese [Zeichenfolge Zellenname] nicht unterstützt wird|
| [import_object_array(obj_array, first_row, first_column, is_vertical)](/cells/de/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool) | Importiert ein Array von Daten in ein Arbeitsblatt.|
| [import_object_array(obj_array, first_row, first_column, is_vertical, skip)](/cells/de/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool-int) | Importiert ein Array von Daten in ein Arbeitsblatt.|
| [import_array(string_array, first_row, first_column, is_vertical)](/cells/de/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importiert ein Array von Zeichenfolgen in ein Arbeitsblatt.|
| [import_array(int_array, first_row, first_column, is_vertical)](/cells/de/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importiert ein Array von Ganzzahlen in ein Arbeitsblatt.|
| [import_array(double_array, first_row, first_column, is_vertical)](/cells/de/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importiert ein Array von Doubles in ein Arbeitsblatt.|
| [import_csv(file_name, splitter, convert_numeric_data, first_row, first_column)](/cells/de/python-net/aspose.cells/cells/import_csv/#str-str-bool-int-int) | Importieren Sie eine CSV-Datei in die Zellen.|
| [import_csv(stream, splitter, convert_numeric_data, first_row, first_column)](/cells/de/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-str-bool-int-int) | Importieren Sie eine CSV-Datei in die Zellen.|
| [import_csv(file_name, options, first_row, first_column)](/cells/de/python-net/aspose.cells/cells/import_csv/#str-TxtLoadOptions-int-int) | Importieren Sie eine CSV-Datei in die Zellen.|
| [import_csv(stream, options, first_row, first_column)](/cells/de/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-TxtLoadOptions-int-int) | Importieren Sie eine CSV-Datei in die Zellen.|
| [merge(first_row, first_column, total_rows, total_columns)](/cells/de/python-net/aspose.cells/cells/merge/#int-int-int-int) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.|
| [merge(first_row, first_column, total_rows, total_columns, merge_conflict)](/cells/de/python-net/aspose.cells/cells/merge/#int-int-int-int-bool) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.|
| [merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict)](/cells/de/python-net/aspose.cells/cells/merge/#int-int-int-int-bool-bool) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number, paste_options)](/cells/de/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-PasteOptions) | Kopiert Daten und Formate einer ganzen Spalte.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number)](/cells/de/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int) | Kopiert Daten und Formate einer ganzen Spalte.|
| [copy_columns(source_cells, source_column_index, source_total_columns, destination_column_index, destination_total_columns)](/cells/de/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-int) | Kopiert Daten und Formate der ganzen Spalten.|
| [copy_rows(source_cells, source_row_index, destination_row_index, row_number)](/cells/de/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int) | Kopiert Daten und Formate einiger ganzer Zeilen.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options)](/cells/de/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions) | Kopiert Daten und Formate einiger ganzer Zeilen.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options, paste_options)](/cells/de/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions-PasteOptions) | Kopiert Daten und Formate einiger ganzer Zeilen.|
| [group_columns(first_index, last_index)](/cells/de/python-net/aspose.cells/cells/group_columns/#int-int) | Spalten gruppieren.|
| [group_columns(first_index, last_index, is_hidden)](/cells/de/python-net/aspose.cells/cells/group_columns/#int-int-bool) | Spalten gruppieren.|
| [ungroup_rows(first_index, last_index, is_all)](/cells/de/python-net/aspose.cells/cells/ungroup_rows/#int-int-bool) | Gruppierung von Zeilen aufheben.|
| [ungroup_rows(first_index, last_index)](/cells/de/python-net/aspose.cells/cells/ungroup_rows/#int-int) | Gruppierung von Zeilen aufheben.|
| [group_rows(first_index, last_index, is_hidden)](/cells/de/python-net/aspose.cells/cells/group_rows/#int-int-bool) | Gruppiert Zeilen.|
| [group_rows(first_index, last_index)](/cells/de/python-net/aspose.cells/cells/group_rows/#int-int) | Gruppiert Zeilen.|
| [delete_column(column_index, update_reference)](/cells/de/python-net/aspose.cells/cells/delete_column/#int-bool) | Löscht eine Spalte.|
| [delete_column(column_index)](/cells/de/python-net/aspose.cells/cells/delete_column/#int) | Löscht eine Spalte.|
| [delete_rows(row_index, total_rows)](/cells/de/python-net/aspose.cells/cells/delete_rows/#int-int) | Löscht mehrere Zeilen.|
| [delete_rows(row_index, total_rows, update_reference)](/cells/de/python-net/aspose.cells/cells/delete_rows/#int-int-bool) | Löscht mehrere Zeilen im Arbeitsblatt.|
| [delete_blank_columns()](/cells/de/python-net/aspose.cells/cells/delete_blank_columns/#) | Löschen Sie alle leeren Spalten, die keine Daten enthalten.|
| [delete_blank_columns(options)](/cells/de/python-net/aspose.cells/cells/delete_blank_columns/#DeleteOptions) | Löschen Sie alle leeren Spalten, die keine Daten enthalten.|
| [delete_blank_rows()](/cells/de/python-net/aspose.cells/cells/delete_blank_rows/#) | Löschen Sie alle leeren Zeilen, die keine Daten enthalten.|
| [delete_blank_rows(options)](/cells/de/python-net/aspose.cells/cells/delete_blank_rows/#DeleteOptions) | Löschen Sie alle leeren Zeilen, die keine Daten enthalten.|
| [insert_columns(column_index, total_columns)](/cells/de/python-net/aspose.cells/cells/insert_columns/#int-int) | Fügt einige Spalten in das Arbeitsblatt ein.|
| [insert_columns(column_index, total_columns, update_reference)](/cells/de/python-net/aspose.cells/cells/insert_columns/#int-int-bool) | Fügt einige Spalten in das Arbeitsblatt ein.|
| [insert_column(column_index, update_reference)](/cells/de/python-net/aspose.cells/cells/insert_column/#int-bool) |Fügt eine neue Spalte in das Arbeitsblatt ein.|
| [insert_column(column_index)](/cells/de/python-net/aspose.cells/cells/insert_column/#int) |Fügt eine neue Spalte in das Arbeitsblatt ein.|
| [insert_rows(row_index, total_rows, update_reference)](/cells/de/python-net/aspose.cells/cells/insert_rows/#int-int-bool) | Fügt mehrere Zeilen in das Arbeitsblatt ein.|
| [insert_rows(row_index, total_rows, options)](/cells/de/python-net/aspose.cells/cells/insert_rows/#int-int-InsertOptions) | Fügt mehrere Zeilen in das Arbeitsblatt ein.|
| [insert_rows(row_index, total_rows)](/cells/de/python-net/aspose.cells/cells/insert_rows/#int-int) | Fügt mehrere Zeilen in das Arbeitsblatt ein.|
| [clear_range(range)](/cells/de/python-net/aspose.cells/cells/clear_range/#CellArea) | Löscht Inhalt und Formatierung eines Bereichs.|
| [clear_range(start_row, start_column, end_row, end_column)](/cells/de/python-net/aspose.cells/cells/clear_range/#int-int-int-int) | Löscht Inhalt und Formatierung eines Bereichs.|
| [clear_contents(range)](/cells/de/python-net/aspose.cells/cells/clear_contents/#CellArea) | Löscht den Inhalt eines Bereichs.|
| [clear_contents(start_row, start_column, end_row, end_column)](/cells/de/python-net/aspose.cells/cells/clear_contents/#int-int-int-int) | Löscht den Inhalt eines Bereichs.|
| [clear_formats(range)](/cells/de/python-net/aspose.cells/cells/clear_formats/#CellArea) | Löscht die Formatierung eines Bereichs.|
| [clear_formats(start_row, start_column, end_row, end_column)](/cells/de/python-net/aspose.cells/cells/clear_formats/#int-int-int-int) | Löscht die Formatierung eines Bereichs.|
| [find(what, previous_cell)](/cells/de/python-net/aspose.cells/cells/find/#any-Cell) | Findet die Zelle, die das Eingabeobjekt enthält.|
| [find(what, previous_cell, find_options)](/cells/de/python-net/aspose.cells/cells/find/#any-Cell-FindOptions) | Findet die Zelle, die das Eingabeobjekt enthält.|
| [end_cell_in_row(row_index)](/cells/de/python-net/aspose.cells/cells/end_cell_in_row/#int) | Ruft die letzte Zelle in dieser Zeile ab.|
| [end_cell_in_row(start_row, end_row, start_column, end_column)](/cells/de/python-net/aspose.cells/cells/end_cell_in_row/#int-int-int-int) | Ruft die letzte Zelle mit maximalem Zeilenindex in diesem Bereich ab.|
| [end_cell_in_column(column_index)](/cells/de/python-net/aspose.cells/cells/end_cell_in_column/#int) | Ruft die letzte Zelle in dieser Spalte ab.|
| [end_cell_in_column(start_row, end_row, start_column, end_column)](/cells/de/python-net/aspose.cells/cells/end_cell_in_column/#int-int-int-int) | Ruft die letzte Zelle mit maximalem Spaltenindex in diesem Bereich ab.|
| [insert_range(area, shift_number, shift_type, update_reference)](/cells/de/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType-bool) | Fügt einen Bereich von Zellen ein und verschiebt Zellen entsprechend der Verschiebeoption.|
| [insert_range(area, shift_type)](/cells/de/python-net/aspose.cells/cells/insert_range/#CellArea-ShiftType) | Fügt einen Bereich von Zellen ein und verschiebt Zellen entsprechend der Verschiebeoption.|
| [insert_range(area, shift_number, shift_type)](/cells/de/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType) | Fügt einen Bereich von Zellen ein und verschiebt Zellen entsprechend der Verschiebeoption.|
| [import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number)](/cells/de/python-net/aspose.cells/cells/import_custom_objects/#list-list-bool-int-int-int-bool-str-bool) | Importiert benutzerdefinierte Objekte.|
| [import_custom_objects(list, first_row, first_column, options)](/cells/de/python-net/aspose.cells/cells/import_custom_objects/#list-int-int-ImportTableOptions) | Importiert benutzerdefinierte Objekte.|
| [subtotal(ca, group_by, function, total_list)](/cells/de/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list) | Erstellt Zwischensummen für den Bereich.|
| [subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data)](/cells/de/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list-bool-bool-bool) | Erstellt Zwischensummen für den Bereich.|
| [remove_duplicates()](/cells/de/python-net/aspose.cells/cells/remove_duplicates/#) | Entfernt doppelte Zeilen im Blatt.|
| [remove_duplicates(start_row, start_column, end_row, end_column)](/cells/de/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int) | Entfernt doppelte Werte im Bereich.|
| [remove_duplicates(start_row, start_column, end_row, end_column, has_headers, column_offsets)](/cells/de/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int-bool-list) | Entfernt doppelte Daten des Bereichs.|
| [get_row_enumerator()](/cells/de/python-net/aspose.cells/cells/get_row_enumerator/#) | Ruft den Zeilenenumerator ab.|
| [get_cell(row, column)](/cells/de/python-net/aspose.cells/cells/get_cell/#int-int) | Ruft das [Cell](/cells/de/python-net/aspose.cells/cell)-Element oder null am angegebenen Zellenzeilenindex und Spaltenindex ab.|
| [get_row(row)](/cells/de/python-net/aspose.cells/cells/get_row/#int) | Ruft das Element [Row](/cells/de/python-net/aspose.cells/row) am angegebenen Zellenzeilenindex ab.|
| [check_cell(row, column)](/cells/de/python-net/aspose.cells/cells/check_cell/#int-int) | Ruft das [Cell](/cells/de/python-net/aspose.cells/cell)-Element oder null am angegebenen Zellenzeilenindex und Spaltenindex ab.|
| [check_row(row)](/cells/de/python-net/aspose.cells/cells/check_row/#int) |Ruft das [Row](/cells/de/python-net/aspose.cells/row)-Element oder den angegebenen Zellenzeilenindex ab.|
| [check_column(column_index)](/cells/de/python-net/aspose.cells/cells/check_column/#int) | Ruft das [Column](/cells/de/python-net/aspose.cells/column)-Element oder null am angegebenen Spaltenindex ab.|
| [is_row_hidden(row_index)](/cells/de/python-net/aspose.cells/cells/is_row_hidden/#int) | Überprüft, ob eine Zeile am angegebenen Index ausgeblendet ist.|
| [is_column_hidden(column_index)](/cells/de/python-net/aspose.cells/cells/is_column_hidden/#int) | Überprüft, ob eine Spalte am angegebenen Index ausgeblendet ist.|
| [add_range(range_object)](/cells/de/python-net/aspose.cells/cells/add_range/#Range) | Fügt Zellen einen Bereichsobjektverweis hinzu|
| [clear()](/cells/de/python-net/aspose.cells/cells/clear/#) | Löscht alle Zellen- und Zeilenobjekte.|
| [import_data(table, first_row, first_column, options)](/cells/de/python-net/aspose.cells/cells/import_data/#ICellsDataTable-int-int-ImportTableOptions) | Importieren Sie Daten aus benutzerdefinierten Datentabellen.|
| [import_array_list(array_list, first_row, first_column, is_vertical)](/cells/de/python-net/aspose.cells/cells/import_array_list/#list-int-int-bool) | Importiert eine Arrayliste von Daten in ein Arbeitsblatt.|
| [import_formula_array(string_array, first_row, first_column, is_vertical)](/cells/de/python-net/aspose.cells/cells/import_formula_array/#list-int-int-bool) | Importiert ein Array von Formeln in ein Arbeitsblatt.|
| [text_to_columns(row, column, total_rows, options)](/cells/de/python-net/aspose.cells/cells/text_to_columns/#int-int-int-TxtLoadOptions) | Teilt den Text in den Spalten in Spalten auf.|
| [un_merge(first_row, first_column, total_rows, total_columns)](/cells/de/python-net/aspose.cells/cells/un_merge/#int-int-int-int) | Hebt die Zusammenführung eines angegebenen Bereichs verbundener Zellen auf.|
| [clear_merged_cells()](/cells/de/python-net/aspose.cells/cells/clear_merged_cells/#) | Löscht alle zusammengeführten Bereiche.|
| [hide_row(row)](/cells/de/python-net/aspose.cells/cells/hide_row/#int) | Blendet eine Zeile aus.|
| [unhide_row(row, height)](/cells/de/python-net/aspose.cells/cells/unhide_row/#int-float) | Eine Zeile einblenden.|
| [hide_rows(row, total_rows)](/cells/de/python-net/aspose.cells/cells/hide_rows/#int-int) | Blendet mehrere Zeilen aus.|
| [unhide_rows(row, total_rows, height)](/cells/de/python-net/aspose.cells/cells/unhide_rows/#int-int-float) | Blendet die ausgeblendeten Zeilen ein.|
| [set_row_height_pixel(row, pixels)](/cells/de/python-net/aspose.cells/cells/set_row_height_pixel/#int-int) | Legt die Zeilenhöhe in Pixeleinheiten fest.|
| [set_row_height_inch(row, inches)](/cells/de/python-net/aspose.cells/cells/set_row_height_inch/#int-float) | Legt die Zeilenhöhe in Einheiten von Zoll fest.|
| [set_row_height(row, height)](/cells/de/python-net/aspose.cells/cells/set_row_height/#int-float) | Legt die Höhe der angegebenen Zeile fest.|
| [get_row_original_height_point(row)](/cells/de/python-net/aspose.cells/cells/get_row_original_height_point/#int) | Ruft die Höhe der ursprünglichen Zeile in Punkteinheiten ab, wenn die Zeile ausgeblendet ist|
| [hide_column(column)](/cells/de/python-net/aspose.cells/cells/hide_column/#int) | Blendet eine Spalte aus.|
| [unhide_column(column, width)](/cells/de/python-net/aspose.cells/cells/unhide_column/#int-float) | Eine Spalte einblenden|
| [hide_columns(column, total_columns)](/cells/de/python-net/aspose.cells/cells/hide_columns/#int-int) | Mehrere Spalten ausblenden.|
| [unhide_columns(column, total_columns, width)](/cells/de/python-net/aspose.cells/cells/unhide_columns/#int-int-float) |Blenden Sie mehrere Spalten ein.|
| [get_row_height(row)](/cells/de/python-net/aspose.cells/cells/get_row_height/#int) | Ruft die Höhe einer angegebenen Zeile ab.|
| [get_view_row_height(row)](/cells/de/python-net/aspose.cells/cells/get_view_row_height/#int) | Ruft die Höhe einer angegebenen Zeile ab.|
| [get_row_height_pixel(row)](/cells/de/python-net/aspose.cells/cells/get_row_height_pixel/#int) | Ruft die Höhe einer angegebenen Zeile in Pixeleinheiten ab.|
| [get_row_height_inch(row)](/cells/de/python-net/aspose.cells/cells/get_row_height_inch/#int) | Ruft die Höhe einer angegebenen Zeile in Einheiten von Zoll ab.|
| [get_view_row_height_inch(row)](/cells/de/python-net/aspose.cells/cells/get_view_row_height_inch/#int) | Ruft die Höhe einer angegebenen Zeile in Einheiten von Zoll ab.|
| [set_column_width_pixel(column, pixels)](/cells/de/python-net/aspose.cells/cells/set_column_width_pixel/#int-int) | Legt die Spaltenbreite in der Einheit Pixel in der Normalansicht fest.|
| [set_column_width_inch(column, inches)](/cells/de/python-net/aspose.cells/cells/set_column_width_inch/#int-float) | Legt die Spaltenbreite in der Einheit Zoll in der Normalansicht fest.|
| [set_column_width(column, width)](/cells/de/python-net/aspose.cells/cells/set_column_width/#int-float) | Legt die Breite der angegebenen Spalte in der Normalansicht fest.|
| [get_column_width_pixel(column)](/cells/de/python-net/aspose.cells/cells/get_column_width_pixel/#int) | Ruft die Breite der angegebenen Spalte in der Normalansicht in Pixeleinheiten ab.|
| [get_column_width_inch(column)](/cells/de/python-net/aspose.cells/cells/get_column_width_inch/#int) | Ruft die Breite der angegebenen Spalte in der Normalansicht in Zoll ab.|
| [get_column_width(column)](/cells/de/python-net/aspose.cells/cells/get_column_width/#int) | Ruft die Breite der angegebenen Spalte in der Normalansicht ab|
| [get_view_column_width_pixel(column)](/cells/de/python-net/aspose.cells/cells/get_view_column_width_pixel/#int) | Holen Sie sich die Breite in verschiedenen Ansichtstypen.|
| [set_view_column_width_pixel(column, pixels)](/cells/de/python-net/aspose.cells/cells/set_view_column_width_pixel/#int-int) | Legt die Breite der Spalte in verschiedenen Ansichten fest.|
| [get_last_data_row(column)](/cells/de/python-net/aspose.cells/cells/get_last_data_row/#int) | Ruft den letzten Zeilenindex der Zelle ab, die Daten in der angegebenen Spalte enthält.|
| [apply_column_style(column, style, flag)](/cells/de/python-net/aspose.cells/cells/apply_column_style/#int-Style-StyleFlag) | Wendet Formate für eine ganze Spalte an.|
| [apply_row_style(row, style, flag)](/cells/de/python-net/aspose.cells/cells/apply_row_style/#int-Style-StyleFlag) | Wendet Formate für eine ganze Zeile an.|
| [apply_style(style, flag)](/cells/de/python-net/aspose.cells/cells/apply_style/#Style-StyleFlag) | Wendet Formate für ein ganzes Arbeitsblatt an.|
| [copy_column(source_cells, source_column_index, destination_column_index)](/cells/de/python-net/aspose.cells/cells/copy_column/#Cells-int-int) | Kopiert Daten und Formate einer ganzen Spalte.|
| [copy_row(source_cells, source_row_index, destination_row_index)](/cells/de/python-net/aspose.cells/cells/copy_row/#Cells-int-int) | Kopiert Daten und Formate einer ganzen Zeile.|
| [get_grouped_row_outline_level(row_index)](/cells/de/python-net/aspose.cells/cells/get_grouped_row_outline_level/#int) |Ruft die Gliederungsebene (nullbasiert) der Zeile ab.|
| [get_grouped_column_outline_level(column_index)](/cells/de/python-net/aspose.cells/cells/get_grouped_column_outline_level/#int) | Ruft die Gliederungsebene (nullbasiert) der Spalte ab.|
| [get_max_grouped_column_outline_level()](/cells/de/python-net/aspose.cells/cells/get_max_grouped_column_outline_level/#) | Ruft die maximale Gliederungsebene der gruppierten Spalte ab (nullbasiert).|
| [get_max_grouped_row_outline_level()](/cells/de/python-net/aspose.cells/cells/get_max_grouped_row_outline_level/#) | Ruft die maximale gruppierte Zeilenumrissebene ab (nullbasiert).|
| [show_group_detail(is_vertical, index)](/cells/de/python-net/aspose.cells/cells/show_group_detail/#bool-int) | Erweitert die gruppierten Zeilen/Spalten.|
| [hide_group_detail(is_vertical, index)](/cells/de/python-net/aspose.cells/cells/hide_group_detail/#bool-int) | Reduziert die gruppierten Zeilen/Spalten.|
| [ungroup_columns(first_index, last_index)](/cells/de/python-net/aspose.cells/cells/ungroup_columns/#int-int) | Hebt die Gruppierung von Spalten auf.|
| [delete_columns(column_index, total_columns, update_reference)](/cells/de/python-net/aspose.cells/cells/delete_columns/#int-int-bool) | Löscht mehrere Spalten.|
| [is_deleting_range_enabled(start_row, start_column, total_rows, total_columns)](/cells/de/python-net/aspose.cells/cells/is_deleting_range_enabled/#int-int-int-int) | Prüfen Sie, ob der Bereich gelöscht werden konnte.|
| [delete_row(row_index)](/cells/de/python-net/aspose.cells/cells/delete_row/#int) | Löscht eine Zeile.|
| [is_blank_column(column_index)](/cells/de/python-net/aspose.cells/cells/is_blank_column/#int) | Überprüft, ob die angegebene Spalte leer ist (keine Daten enthält).|
| [insert_row(row_index)](/cells/de/python-net/aspose.cells/cells/insert_row/#int) | Fügt eine neue Zeile in das Arbeitsblatt ein.|
| [link_to_xml_map(map_name, row, column, path)](/cells/de/python-net/aspose.cells/cells/link_to_xml_map/#str-int-int-str) | Link zu einer XML-Karte.|
| [find_formula(formula, previous_cell)](/cells/de/python-net/aspose.cells/cells/find_formula/#str-Cell) | Findet die Zelle mit der Eingabezeichenfolge.|
| [find_formula_contains(formula, previous_cell)](/cells/de/python-net/aspose.cells/cells/find_formula_contains/#str-Cell) | Findet die Zelle mit der Formel, die die Eingabezeichenfolge enthält.|
| [move_range(source_area, dest_row, dest_column)](/cells/de/python-net/aspose.cells/cells/move_range/#CellArea-int-int) | Verschiebt den Bereich.|
| [insert_cut_cells(cut_range, row, column, shift_type)](/cells/de/python-net/aspose.cells/cells/insert_cut_cells/#Range-int-int-ShiftType) | Schnittbereich einfügen.|
| [delete_range(start_row, start_column, end_row, end_column, shift_type)](/cells/de/python-net/aspose.cells/cells/delete_range/#int-int-int-int-ShiftType) | Löscht einen Bereich von Zellen und verschiebt Zellen entsprechend der Verschiebeoption.|
| [retrieve_subtotal_setting(ca)](/cells/de/python-net/aspose.cells/cells/retrieve_subtotal_setting/#CellArea) | Ruft die Zwischensummeneinstellung des Bereichs ab.|
| [remove_formulas()](/cells/de/python-net/aspose.cells/cells/remove_formulas/#) | Entfernt alle Formeln und ersetzt sie durch den Wert der Formel.|
| [convert_string_to_numeric_value()](/cells/de/python-net/aspose.cells/cells/convert_string_to_numeric_value/#) |Konvertiert Zeichenfolgendaten in Zellen nach Möglichkeit in numerische Werte.|
| [get_dependents(is_all, row, column)](/cells/de/python-net/aspose.cells/cells/get_dependents/#bool-int-int) | Holen Sie sich alle Zellen, die sich auf die bestimmte Zelle beziehen.|
| [get_dependents_in_calculation(row, column, recursive)](/cells/de/python-net/aspose.cells/cells/get_dependents_in_calculation/#int-int-bool) | Ruft alle Zellen ab, deren berechnetes Ergebnis von bestimmten Zellen abhängt.|
| [get_cell_style(row, column)](/cells/de/python-net/aspose.cells/cells/get_cell_style/#int-int) | Holen Sie sich den Stil der angegebenen Zelle.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
* Klasse [Column](/cells/de/python-net/aspose.cells/column)
* Klasse [Range](/cells/de/python-net/aspose.cells/range)
* Klasse [Row](/cells/de/python-net/aspose.cells/row)
