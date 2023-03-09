---
title: classe Cells
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 180
url: /it/python-net/aspose.cells/cells/
is_root: false
---
##  classe Cells
Incapsula una raccolta di oggetti rilevanti per la cella, come [Cell](/cells/it/python-net/aspose.cells/cell), [Row](/cells/it/python-net/aspose.cells/row), ...ecc.



Il tipo Cells espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [ods_cell_fields](/cells/it/python-net/aspose.cells/cells/ods_cell_fields) |Ottiene l'elenco dei campi di ods.|
| [count](/cells/it/python-net/aspose.cells/cells/count) | Ottiene il conteggio totale degli oggetti Cell di cui è stata creata un'istanza.|
| [count_large](/cells/it/python-net/aspose.cells/cells/count_large) | Ottiene il conteggio totale degli oggetti Cell di cui è stata creata un'istanza.|
| [rows](/cells/it/python-net/aspose.cells/cells/rows) | Ottiene la raccolta di oggetti [Row](/cells/it/python-net/aspose.cells/row) che rappresenta le singole righe in questo foglio di lavoro.|
| [merged_cells](/cells/it/python-net/aspose.cells/cells/merged_cells) | Ottiene la raccolta di celle unite.|
| [multi_thread_reading](/cells/it/python-net/aspose.cells/cells/multi_thread_reading) | Ottiene o imposta se il modello di dati delle celle deve supportare la lettura multithread.<br/> Il valore predefinito di questa proprietà è false.|
| [memory_setting](/cells/it/python-net/aspose.cells/cells/memory_setting) | Ottiene o imposta l'opzione di utilizzo della memoria per queste celle.|
| [style](/cells/it/python-net/aspose.cells/cells/style) | Ottiene e imposta lo stile predefinito.|
| [standard_width_inch](/cells/it/python-net/aspose.cells/cells/standard_width_inch) | Ottiene o imposta la larghezza della colonna predefinita nel foglio di lavoro, in unità di pollici.|
| [standard_width_pixels](/cells/it/python-net/aspose.cells/cells/standard_width_pixels) | Ottiene o imposta la larghezza della colonna predefinita nel foglio di lavoro, in unità di pixel.|
| [standard_width](/cells/it/python-net/aspose.cells/cells/standard_width) | Ottiene o imposta la larghezza predefinita della colonna nel foglio di lavoro, in unità di caratteri.|
| [standard_height](/cells/it/python-net/aspose.cells/cells/standard_height) | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di punti.|
| [standard_height_pixels](/cells/it/python-net/aspose.cells/cells/standard_height_pixels) | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di pixel.|
| [standard_height_inch](/cells/it/python-net/aspose.cells/cells/standard_height_inch) | Ottiene o imposta l'altezza della riga predefinita in questo foglio di lavoro, in unità di pollici.|
| [preserve_string](/cells/it/python-net/aspose.cells/cells/preserve_string) | Ottiene o imposta un valore che indica se tutti i valori del foglio di lavoro vengono mantenuti come stringhe.<br/> L'impostazione predefinita è false.|
| [min_row](/cells/it/python-net/aspose.cells/cells/min_row) | Indice di riga minimo della cella che contiene dati o stile.|
| [max_row](/cells/it/python-net/aspose.cells/cells/max_row) | Indice di riga massimo della cella che contiene dati o stile.|
| [min_column](/cells/it/python-net/aspose.cells/cells/min_column) | Indice di colonna minimo di quelle celle che sono state istanziate nella raccolta (non include la colonna<br/>dove style è definito per l'intera colonna ma nessuna cella è stata istanziata in essa).|
| [max_column](/cells/it/python-net/aspose.cells/cells/max_column) | Indice di colonna minimo di quelle celle che sono state istanziate nella raccolta (non include la colonna<br/>dove style è definito per l'intera colonna ma nessuna cella è stata istanziata in essa).|
| [min_data_row](/cells/it/python-net/aspose.cells/cells/min_data_row) | Indice di riga minimo della cella che contiene i dati.|
| [max_data_row](/cells/it/python-net/aspose.cells/cells/max_data_row) | Indice di riga massimo della cella che contiene i dati.|
| [min_data_column](/cells/it/python-net/aspose.cells/cells/min_data_column) | Indice di colonna minimo della cella che contiene i dati.|
| [max_data_column](/cells/it/python-net/aspose.cells/cells/max_data_column) | Indice di colonna massimo della cella che contiene i dati.|
| [is_default_row_height_matched](/cells/it/python-net/aspose.cells/cells/is_default_row_height_matched) | Indica che l'altezza della riga e l'altezza predefinita del carattere corrispondono|
| [is_default_row_hidden](/cells/it/python-net/aspose.cells/cells/is_default_row_hidden) | Indica se la riga è nascosta per impostazione predefinita.|
| [columns](/cells/it/python-net/aspose.cells/cells/columns) | Ottiene la raccolta di oggetti [Column](/cells/it/python-net/aspose.cells/column) che rappresenta le singole colonne in questo foglio di lavoro.|
| [ranges](/cells/it/python-net/aspose.cells/cells/ranges) | Ottiene la raccolta di oggetti [Range](/cells/it/python-net/aspose.cells/range) creati in fase di esecuzione.|
| [last_cell](/cells/it/python-net/aspose.cells/cells/last_cell) | Ottiene l'ultima cella in questo foglio di lavoro.|
| [max_display_range](/cells/it/python-net/aspose.cells/cells/max_display_range) | Ottiene l'intervallo massimo che include dati, celle unite e forme.|
| [first_cell](/cells/it/python-net/aspose.cells/cells/first_cell) | Ottiene la prima cella in questo foglio di lavoro.|



Ottiene l'elemento [Cell](/cells/it/python-net/aspose.cells/cell) all'interno del foglio di lavoro
###  Indicizzatore
| Nome| Descrizione|
| :- | :- |
| [index] | L'indice in base zero dell'elemento.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [create_range(upper_left_cell, lower_right_cell)](/cells/it/python-net/aspose.cells/cells/create_range/#str-str) | Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da un intervallo di celle.|
| [create_range(first_row, first_column, total_rows, total_columns)](/cells/it/python-net/aspose.cells/cells/create_range/#int-int-int-int) | Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da un intervallo di celle.|
| [create_range(address)](/cells/it/python-net/aspose.cells/cells/create_range/#str) | Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da un indirizzo dell'intervallo.|
| [create_range(first_index, number, is_vertical)](/cells/it/python-net/aspose.cells/cells/create_range/#int-int-bool) | Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da righe di celle o colonne di celle.|
| [get(row, column)](/cells/it/python-net/aspose.cells/cells/get/#int-int) | Aggiungi API for Python tramite .Net.poiché questo[int row, int column] non è supportato|
| [get(cell_name)](/cells/it/python-net/aspose.cells/cells/get/#str) | Aggiungi API for Python tramite .Net.poiché this[string cellName] non è supportato|
| [import_object_array(obj_array, first_row, first_column, is_vertical)](/cells/it/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool) | Importa una matrice di dati in un foglio di lavoro.|
| [import_object_array(obj_array, first_row, first_column, is_vertical, skip)](/cells/it/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool-int) | Importa una matrice di dati in un foglio di lavoro.|
| [import_array(string_array, first_row, first_column, is_vertical)](/cells/it/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importa una matrice di stringhe in un foglio di lavoro.|
| [import_array(int_array, first_row, first_column, is_vertical)](/cells/it/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importa una matrice di numeri interi in un foglio di lavoro.|
| [import_array(double_array, first_row, first_column, is_vertical)](/cells/it/python-net/aspose.cells/cells/import_array/#list-int-int-bool) | Importa una matrice di double in un foglio di lavoro.|
| [import_csv(file_name, splitter, convert_numeric_data, first_row, first_column)](/cells/it/python-net/aspose.cells/cells/import_csv/#str-str-bool-int-int) | Importa un file CSV nelle celle.|
| [import_csv(stream, splitter, convert_numeric_data, first_row, first_column)](/cells/it/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-str-bool-int-int) | Importa un file CSV nelle celle.|
| [import_csv(file_name, options, first_row, first_column)](/cells/it/python-net/aspose.cells/cells/import_csv/#str-TxtLoadOptions-int-int) | Importa un file CSV nelle celle.|
| [import_csv(stream, options, first_row, first_column)](/cells/it/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-TxtLoadOptions-int-int) | Importa un file CSV nelle celle.|
| [merge(first_row, first_column, total_rows, total_columns)](/cells/it/python-net/aspose.cells/cells/merge/#int-int-int-int) | Unisce un intervallo di celle specificato in una singola cella.|
| [merge(first_row, first_column, total_rows, total_columns, merge_conflict)](/cells/it/python-net/aspose.cells/cells/merge/#int-int-int-int-bool) | Unisce un intervallo di celle specificato in una singola cella.|
| [merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict)](/cells/it/python-net/aspose.cells/cells/merge/#int-int-int-int-bool-bool) | Unisce un intervallo di celle specificato in una singola cella.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number, paste_options)](/cells/it/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-PasteOptions) | Copia dati e formati di un'intera colonna.|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number)](/cells/it/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int) | Copia dati e formati di un'intera colonna.|
| [copy_columns(source_cells, source_column_index, source_total_columns, destination_column_index, destination_total_columns)](/cells/it/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-int) | Copia dati e formati di intere colonne.|
| [copy_rows(source_cells, source_row_index, destination_row_index, row_number)](/cells/it/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int) | Copia dati e formati di alcune intere righe.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options)](/cells/it/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions) | Copia dati e formati di alcune intere righe.|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options, paste_options)](/cells/it/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions-PasteOptions) | Copia dati e formati di alcune intere righe.|
| [group_columns(first_index, last_index)](/cells/it/python-net/aspose.cells/cells/group_columns/#int-int) | Colonne dei gruppi.|
| [group_columns(first_index, last_index, is_hidden)](/cells/it/python-net/aspose.cells/cells/group_columns/#int-int-bool) | Colonne dei gruppi.|
| [ungroup_rows(first_index, last_index, is_all)](/cells/it/python-net/aspose.cells/cells/ungroup_rows/#int-int-bool) | Separa le righe.|
| [ungroup_rows(first_index, last_index)](/cells/it/python-net/aspose.cells/cells/ungroup_rows/#int-int) | Separa le righe.|
| [group_rows(first_index, last_index, is_hidden)](/cells/it/python-net/aspose.cells/cells/group_rows/#int-int-bool) | Righe di gruppi.|
| [group_rows(first_index, last_index)](/cells/it/python-net/aspose.cells/cells/group_rows/#int-int) | Righe di gruppi.|
| [delete_column(column_index, update_reference)](/cells/it/python-net/aspose.cells/cells/delete_column/#int-bool) | Elimina una colonna.|
| [delete_column(column_index)](/cells/it/python-net/aspose.cells/cells/delete_column/#int) | Elimina una colonna.|
| [delete_rows(row_index, total_rows)](/cells/it/python-net/aspose.cells/cells/delete_rows/#int-int) | Elimina diverse righe.|
| [delete_rows(row_index, total_rows, update_reference)](/cells/it/python-net/aspose.cells/cells/delete_rows/#int-int-bool) | Elimina più righe nel foglio di lavoro.|
| [delete_blank_columns()](/cells/it/python-net/aspose.cells/cells/delete_blank_columns/#) | Elimina tutte le colonne vuote che non contengono dati.|
| [delete_blank_columns(options)](/cells/it/python-net/aspose.cells/cells/delete_blank_columns/#DeleteOptions) | Elimina tutte le colonne vuote che non contengono dati.|
| [delete_blank_rows()](/cells/it/python-net/aspose.cells/cells/delete_blank_rows/#) |Elimina tutte le righe vuote che non contengono dati.|
| [delete_blank_rows(options)](/cells/it/python-net/aspose.cells/cells/delete_blank_rows/#DeleteOptions) |Elimina tutte le righe vuote che non contengono dati.|
| [insert_columns(column_index, total_columns)](/cells/it/python-net/aspose.cells/cells/insert_columns/#int-int) | Inserisce alcune colonne nel foglio di lavoro.|
| [insert_columns(column_index, total_columns, update_reference)](/cells/it/python-net/aspose.cells/cells/insert_columns/#int-int-bool) | Inserisce alcune colonne nel foglio di lavoro.|
| [insert_column(column_index, update_reference)](/cells/it/python-net/aspose.cells/cells/insert_column/#int-bool) | Inserisce una nuova colonna nel foglio di lavoro.|
| [insert_column(column_index)](/cells/it/python-net/aspose.cells/cells/insert_column/#int) | Inserisce una nuova colonna nel foglio di lavoro.|
| [insert_rows(row_index, total_rows, update_reference)](/cells/it/python-net/aspose.cells/cells/insert_rows/#int-int-bool) | Inserisce più righe nel foglio di lavoro.|
| [insert_rows(row_index, total_rows, options)](/cells/it/python-net/aspose.cells/cells/insert_rows/#int-int-InsertOptions) | Inserisce più righe nel foglio di lavoro.|
| [insert_rows(row_index, total_rows)](/cells/it/python-net/aspose.cells/cells/insert_rows/#int-int) | Inserisce più righe nel foglio di lavoro.|
| [clear_range(range)](/cells/it/python-net/aspose.cells/cells/clear_range/#CellArea) | Cancella il contenuto e la formattazione di un intervallo.|
| [clear_range(start_row, start_column, end_row, end_column)](/cells/it/python-net/aspose.cells/cells/clear_range/#int-int-int-int) | Cancella il contenuto e la formattazione di un intervallo.|
| [clear_contents(range)](/cells/it/python-net/aspose.cells/cells/clear_contents/#CellArea) | Cancella il contenuto di un intervallo.|
| [clear_contents(start_row, start_column, end_row, end_column)](/cells/it/python-net/aspose.cells/cells/clear_contents/#int-int-int-int) | Cancella il contenuto di un intervallo.|
| [clear_formats(range)](/cells/it/python-net/aspose.cells/cells/clear_formats/#CellArea) | Cancella la formattazione di un intervallo.|
| [clear_formats(start_row, start_column, end_row, end_column)](/cells/it/python-net/aspose.cells/cells/clear_formats/#int-int-int-int) | Cancella la formattazione di un intervallo.|
| [find(what, previous_cell)](/cells/it/python-net/aspose.cells/cells/find/#any-Cell) | Trova la cella contenente l'oggetto di input.|
| [find(what, previous_cell, find_options)](/cells/it/python-net/aspose.cells/cells/find/#any-Cell-FindOptions) | Trova la cella contenente l'oggetto di input.|
| [end_cell_in_row(row_index)](/cells/it/python-net/aspose.cells/cells/end_cell_in_row/#int) | Ottiene l'ultima cella in questa riga.|
| [end_cell_in_row(start_row, end_row, start_column, end_column)](/cells/it/python-net/aspose.cells/cells/end_cell_in_row/#int-int-int-int) | Ottiene l'ultima cella con il massimo indice di riga in questo intervallo.|
| [end_cell_in_column(column_index)](/cells/it/python-net/aspose.cells/cells/end_cell_in_column/#int) | Ottiene l'ultima cella in questa colonna.|
| [end_cell_in_column(start_row, end_row, start_column, end_column)](/cells/it/python-net/aspose.cells/cells/end_cell_in_column/#int-int-int-int) | Ottiene l'ultima cella con l'indice di colonna massimo in questo intervallo.|
| [insert_range(area, shift_number, shift_type, update_reference)](/cells/it/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType-bool) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento.|
| [insert_range(area, shift_type)](/cells/it/python-net/aspose.cells/cells/insert_range/#CellArea-ShiftType) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento.|
| [insert_range(area, shift_number, shift_type)](/cells/it/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType) | Inserisce un intervallo di celle e sposta le celle in base all'opzione di spostamento.|
| [import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number)](/cells/it/python-net/aspose.cells/cells/import_custom_objects/#list-list-bool-int-int-int-bool-str-bool) | Importa oggetti personalizzati.|
| [import_custom_objects(list, first_row, first_column, options)](/cells/it/python-net/aspose.cells/cells/import_custom_objects/#list-int-int-ImportTableOptions) | Importa oggetti personalizzati.|
| [subtotal(ca, group_by, function, total_list)](/cells/it/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list) | Crea subtotali per l'intervallo.|
| [subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data)](/cells/it/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list-bool-bool-bool) | Crea subtotali per l'intervallo.|
| [remove_duplicates()](/cells/it/python-net/aspose.cells/cells/remove_duplicates/#) | Rimuove le righe duplicate nel foglio.|
| [remove_duplicates(start_row, start_column, end_row, end_column)](/cells/it/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int) | Rimuove i valori duplicati nell'intervallo.|
| [remove_duplicates(start_row, start_column, end_row, end_column, has_headers, column_offsets)](/cells/it/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int-bool-list) | Rimuove i dati duplicati dell'intervallo.|
| [get_row_enumerator()](/cells/it/python-net/aspose.cells/cells/get_row_enumerator/#) | Ottiene l'enumeratore di righe.|
| [get_cell(row, column)](/cells/it/python-net/aspose.cells/cells/get_cell/#int-int) | Ottiene l'elemento [Cell](/cells/it/python-net/aspose.cells/cell) o null in corrispondenza dell'indice di riga della cella e dell'indice di colonna specificati.|
| [get_row(row)](/cells/it/python-net/aspose.cells/cells/get_row/#int) |Ottiene l'elemento [Row](/cells/it/python-net/aspose.cells/row) in corrispondenza dell'indice di riga della cella specificato.|
| [check_cell(row, column)](/cells/it/python-net/aspose.cells/cells/check_cell/#int-int) | Ottiene l'elemento [Cell](/cells/it/python-net/aspose.cells/cell) o null in corrispondenza dell'indice di riga della cella e dell'indice di colonna specificati.|
| [check_row(row)](/cells/it/python-net/aspose.cells/cells/check_row/#int) | Ottiene l'elemento [Row](/cells/it/python-net/aspose.cells/row) o l'indice di riga della cella specificato.|
| [check_column(column_index)](/cells/it/python-net/aspose.cells/cells/check_column/#int) | Ottiene l'elemento [Column](/cells/it/python-net/aspose.cells/column) o null in corrispondenza dell'indice di colonna specificato.|
| [is_row_hidden(row_index)](/cells/it/python-net/aspose.cells/cells/is_row_hidden/#int) | Controlla se una riga in corrispondenza di un determinato indice è nascosta.|
| [is_column_hidden(column_index)](/cells/it/python-net/aspose.cells/cells/is_column_hidden/#int) | Controlla se una colonna in un determinato indice è nascosta.|
| [add_range(range_object)](/cells/it/python-net/aspose.cells/cells/add_range/#Range) | Aggiunge un riferimento all'oggetto intervallo alle celle|
| [clear()](/cells/it/python-net/aspose.cells/cells/clear/#) | Cancella tutti gli oggetti cella e riga.|
| [import_data(table, first_row, first_column, options)](/cells/it/python-net/aspose.cells/cells/import_data/#ICellsDataTable-int-int-ImportTableOptions) | Importa i dati dalla tabella dati personalizzata.|
| [import_array_list(array_list, first_row, first_column, is_vertical)](/cells/it/python-net/aspose.cells/cells/import_array_list/#list-int-int-bool) | Importa un elenco di matrici di dati in un foglio di lavoro.|
| [import_formula_array(string_array, first_row, first_column, is_vertical)](/cells/it/python-net/aspose.cells/cells/import_formula_array/#list-int-int-bool) | Importa una matrice di formule in un foglio di lavoro.|
| [text_to_columns(row, column, total_rows, options)](/cells/it/python-net/aspose.cells/cells/text_to_columns/#int-int-int-TxtLoadOptions) | Divide il testo nella colonna in colonne.|
| [un_merge(first_row, first_column, total_rows, total_columns)](/cells/it/python-net/aspose.cells/cells/un_merge/#int-int-int-int) | Separa un intervallo specificato di celle unite.|
| [clear_merged_cells()](/cells/it/python-net/aspose.cells/cells/clear_merged_cells/#) | Cancella tutti gli intervalli uniti.|
| [hide_row(row)](/cells/it/python-net/aspose.cells/cells/hide_row/#int) | Nasconde una riga.|
| [unhide_row(row, height)](/cells/it/python-net/aspose.cells/cells/unhide_row/#int-float) | Mostra una riga.|
| [hide_rows(row, total_rows)](/cells/it/python-net/aspose.cells/cells/hide_rows/#int-int) | Nasconde più righe.|
| [unhide_rows(row, total_rows, height)](/cells/it/python-net/aspose.cells/cells/unhide_rows/#int-int-float) | Mostra le righe nascoste.|
| [set_row_height_pixel(row, pixels)](/cells/it/python-net/aspose.cells/cells/set_row_height_pixel/#int-int) | Imposta l'altezza della riga in unità di pixel.|
| [set_row_height_inch(row, inches)](/cells/it/python-net/aspose.cells/cells/set_row_height_inch/#int-float) | Imposta l'altezza della riga in unità di pollici.|
| [set_row_height(row, height)](/cells/it/python-net/aspose.cells/cells/set_row_height/#int-float) | Imposta l'altezza della riga specificata.|
| [get_row_original_height_point(row)](/cells/it/python-net/aspose.cells/cells/get_row_original_height_point/#int) | Ottiene l'altezza della riga originale in unità di punti se la riga è nascosta|
| [hide_column(column)](/cells/it/python-net/aspose.cells/cells/hide_column/#int) | Nasconde una colonna.|
| [unhide_column(column, width)](/cells/it/python-net/aspose.cells/cells/unhide_column/#int-float) | Mostra una colonna|
| [hide_columns(column, total_columns)](/cells/it/python-net/aspose.cells/cells/hide_columns/#int-int) | Nascondi più colonne.|
| [unhide_columns(column, total_columns, width)](/cells/it/python-net/aspose.cells/cells/unhide_columns/#int-int-float) | Scopri più colonne.|
| [get_row_height(row)](/cells/it/python-net/aspose.cells/cells/get_row_height/#int) | Ottiene l'altezza di una riga specificata.|
| [get_view_row_height(row)](/cells/it/python-net/aspose.cells/cells/get_view_row_height/#int) | Ottiene l'altezza di una riga specificata.|
| [get_row_height_pixel(row)](/cells/it/python-net/aspose.cells/cells/get_row_height_pixel/#int) | Ottiene l'altezza di una riga specificata in unità di pixel.|
| [get_row_height_inch(row)](/cells/it/python-net/aspose.cells/cells/get_row_height_inch/#int) | Ottiene l'altezza di una riga specificata in pollici.|
| [get_view_row_height_inch(row)](/cells/it/python-net/aspose.cells/cells/get_view_row_height_inch/#int) | Ottiene l'altezza di una riga specificata in pollici.|
| [set_column_width_pixel(column, pixels)](/cells/it/python-net/aspose.cells/cells/set_column_width_pixel/#int-int) | Imposta la larghezza della colonna in unità di pixel nella visualizzazione normale.|
| [set_column_width_inch(column, inches)](/cells/it/python-net/aspose.cells/cells/set_column_width_inch/#int-float) | Imposta la larghezza della colonna in unità di pollici nella visualizzazione normale.|
| [set_column_width(column, width)](/cells/it/python-net/aspose.cells/cells/set_column_width/#int-float) | Imposta la larghezza della colonna specificata nella visualizzazione normale.|
| [get_column_width_pixel(column)](/cells/it/python-net/aspose.cells/cells/get_column_width_pixel/#int) | Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pixel.|
| [get_column_width_inch(column)](/cells/it/python-net/aspose.cells/cells/get_column_width_inch/#int) | Ottiene la larghezza della colonna specificata nella visualizzazione normale, in unità di pollici.|
| [get_column_width(column)](/cells/it/python-net/aspose.cells/cells/get_column_width/#int) | Ottiene la larghezza della colonna specificata nella visualizzazione normale|
| [get_view_column_width_pixel(column)](/cells/it/python-net/aspose.cells/cells/get_view_column_width_pixel/#int) | Ottieni la larghezza in diversi tipi di visualizzazione.|
| [set_view_column_width_pixel(column, pixels)](/cells/it/python-net/aspose.cells/cells/set_view_column_width_pixel/#int-int) | Imposta la larghezza della colonna in una vista diversa.|
| [get_last_data_row(column)](/cells/it/python-net/aspose.cells/cells/get_last_data_row/#int) |Ottiene l'indice dell'ultima riga della cella che contiene i dati nella colonna specificata.|
| [apply_column_style(column, style, flag)](/cells/it/python-net/aspose.cells/cells/apply_column_style/#int-Style-StyleFlag) | Applica i formati per un'intera colonna.|
| [apply_row_style(row, style, flag)](/cells/it/python-net/aspose.cells/cells/apply_row_style/#int-Style-StyleFlag) | Applica i formati per un'intera riga.|
| [apply_style(style, flag)](/cells/it/python-net/aspose.cells/cells/apply_style/#Style-StyleFlag) |Applica i formati per un intero foglio di lavoro.|
| [copy_column(source_cells, source_column_index, destination_column_index)](/cells/it/python-net/aspose.cells/cells/copy_column/#Cells-int-int) | Copia dati e formati di un'intera colonna.|
| [copy_row(source_cells, source_row_index, destination_row_index)](/cells/it/python-net/aspose.cells/cells/copy_row/#Cells-int-int) | Copia dati e formati di un'intera riga.|
| [get_grouped_row_outline_level(row_index)](/cells/it/python-net/aspose.cells/cells/get_grouped_row_outline_level/#int) | Ottiene il livello struttura (in base zero) della riga.|
| [get_grouped_column_outline_level(column_index)](/cells/it/python-net/aspose.cells/cells/get_grouped_column_outline_level/#int) | Ottiene il livello struttura (in base zero) della colonna.|
| [get_max_grouped_column_outline_level()](/cells/it/python-net/aspose.cells/cells/get_max_grouped_column_outline_level/#) | Ottiene il massimo livello di struttura della colonna raggruppata (in base zero).|
| [get_max_grouped_row_outline_level()](/cells/it/python-net/aspose.cells/cells/get_max_grouped_row_outline_level/#) | Ottiene il massimo livello di struttura delle righe raggruppate (in base zero).|
| [show_group_detail(is_vertical, index)](/cells/it/python-net/aspose.cells/cells/show_group_detail/#bool-int) | Espande le righe/colonne raggruppate.|
| [hide_group_detail(is_vertical, index)](/cells/it/python-net/aspose.cells/cells/hide_group_detail/#bool-int) | Comprime le righe/colonne raggruppate.|
| [ungroup_columns(first_index, last_index)](/cells/it/python-net/aspose.cells/cells/ungroup_columns/#int-int) | Separa le colonne.|
| [delete_columns(column_index, total_columns, update_reference)](/cells/it/python-net/aspose.cells/cells/delete_columns/#int-int-bool) | Elimina diverse colonne.|
| [is_deleting_range_enabled(start_row, start_column, total_rows, total_columns)](/cells/it/python-net/aspose.cells/cells/is_deleting_range_enabled/#int-int-int-int) | Controlla se è possibile eliminare l'intervallo.|
| [delete_row(row_index)](/cells/it/python-net/aspose.cells/cells/delete_row/#int) | Elimina una riga.|
| [is_blank_column(column_index)](/cells/it/python-net/aspose.cells/cells/is_blank_column/#int) | Controlla se la colonna specificata è vuota (non contiene dati).|
| [insert_row(row_index)](/cells/it/python-net/aspose.cells/cells/insert_row/#int) | Inserisce una nuova riga nel foglio di lavoro.|
| [link_to_xml_map(map_name, row, column, path)](/cells/it/python-net/aspose.cells/cells/link_to_xml_map/#str-int-int-str) | Collegamento a una mappa xml.|
| [find_formula(formula, previous_cell)](/cells/it/python-net/aspose.cells/cells/find_formula/#str-Cell) | Trova la cella con la stringa di input.|
| [find_formula_contains(formula, previous_cell)](/cells/it/python-net/aspose.cells/cells/find_formula_contains/#str-Cell) | Trova la cella con la formula che contiene la stringa di input.|
| [move_range(source_area, dest_row, dest_column)](/cells/it/python-net/aspose.cells/cells/move_range/#CellArea-int-int) | Sposta l'intervallo.|
| [insert_cut_cells(cut_range, row, column, shift_type)](/cells/it/python-net/aspose.cells/cells/insert_cut_cells/#Range-int-int-ShiftType) | Inserisci intervallo di taglio.|
| [delete_range(start_row, start_column, end_row, end_column, shift_type)](/cells/it/python-net/aspose.cells/cells/delete_range/#int-int-int-int-ShiftType) | Elimina un intervallo di celle e sposta le celle in base all'opzione di spostamento.|
| [retrieve_subtotal_setting(ca)](/cells/it/python-net/aspose.cells/cells/retrieve_subtotal_setting/#CellArea) | Recupera l'impostazione dei subtotali dell'intervallo.|
| [remove_formulas()](/cells/it/python-net/aspose.cells/cells/remove_formulas/#) |Rimuove tutte le formule e le sostituisce con il valore della formula.|
| [convert_string_to_numeric_value()](/cells/it/python-net/aspose.cells/cells/convert_string_to_numeric_value/#) | Converte i dati stringa nelle celle in valori numerici, se possibile.|
| [get_dependents(is_all, row, column)](/cells/it/python-net/aspose.cells/cells/get_dependents/#bool-int-int) | Ottieni tutte le celle che fanno riferimento alla cella specifica.|
| [get_dependents_in_calculation(row, column, recursive)](/cells/it/python-net/aspose.cells/cells/get_dependents_in_calculation/#int-int-bool) | Ottiene tutte le celle il cui risultato calcolato dipende da una cella specifica.|
| [get_cell_style(row, column)](/cells/it/python-net/aspose.cells/cells/get_cell_style/#int-int) | Ottieni lo stile di una data cella.|



###  Guarda anche
* modulo [aspose.cells](..)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)
* classe [Column](/cells/it/python-net/aspose.cells/column)
* classe [Range](/cells/it/python-net/aspose.cells/range)
* classe [Row](/cells/it/python-net/aspose.cells/row)
