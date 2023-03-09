---
title: classe PivotTable
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 100
url: /it/python-net/aspose.cells.pivot/pivottable/
is_root: false
---
##  classe PivotTable
Descrizione sintetica per PivotTable.



Il tipo PivotTable espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [is_excel_2003_compatible](/cells/it/python-net/aspose.cells.pivot/pivottable/is_excel_2003_compatible) | Specifica se la tabella pivot è compatibile con Excel2003 durante l'aggiornamento della tabella pivot,<br/>se vero, una stringa deve essere minore o uguale a 255 caratteri, quindi se la stringa è maggiore di 255 caratteri,<br/>verrà troncato.se falso, una stringa non avrà la suddetta restrizione.<br/> Il valore predefinito è true.|
| [refreshed_by_who](/cells/it/python-net/aspose.cells.pivot/pivottable/refreshed_by_who) | Ottiene il nome dell'utente che ha aggiornato per ultimo la tabella pivot|
| [refresh_date](/cells/it/python-net/aspose.cells.pivot/pivottable/refresh_date) | Ottiene la data dell'ultimo aggiornamento della tabella pivot.|
| [pivot_table_style_name](/cells/it/python-net/aspose.cells.pivot/pivottable/pivot_table_style_name) | Ottiene e imposta il nome dello stile della tabella pivot.|
| [pivot_table_style_type](/cells/it/python-net/aspose.cells.pivot/pivottable/pivot_table_style_type) | Ottiene e imposta lo stile della tabella pivot predefinito.|
| [column_fields](/cells/it/python-net/aspose.cells.pivot/pivottable/column_fields) | Restituisce un oggetto PivotFields attualmente visualizzato come campi colonna.|
| [row_fields](/cells/it/python-net/aspose.cells.pivot/pivottable/row_fields) | Restituisce un oggetto PivotFields attualmente visualizzato come campi riga.|
| [page_fields](/cells/it/python-net/aspose.cells.pivot/pivottable/page_fields) | Restituisce un oggetto PivotFields attualmente visualizzato come campi di pagina.|
| [data_fields](/cells/it/python-net/aspose.cells.pivot/pivottable/data_fields) | Ottiene un oggetto PivotField che rappresenta tutti i campi dati in una tabella pivot.<br/>Sola lettura Sarebbe init solo quando ci sono due o più campi dati nei DataPiovtFields.<br/>Usa solo per aggiungere DataPivotField all'area riga/colonna della tabella pivot.L'impostazione predefinita è nell'area riga.|
| [data_field](/cells/it/python-net/aspose.cells.pivot/pivottable/data_field) | Ottiene un oggetto PivotField che rappresenta tutti i campi dati in una tabella pivot.<br/>Sola lettura Sarebbe init solo quando ci sono due o più campi dati nei DataPiovtFields.<br/>Usa solo per aggiungere DataPivotField all'area riga/colonna della tabella pivot.L'impostazione predefinita è nell'area riga.|
| [base_fields](/cells/it/python-net/aspose.cells.pivot/pivottable/base_fields) | Restituisce un oggetto PivotFields che include tutti i campi nel rapporto di tabella pivot|
| [pivot_filters](/cells/it/python-net/aspose.cells.pivot/pivottable/pivot_filters) | Restituisce un oggetto PivotFilterCollection.|
| [column_range](/cells/it/python-net/aspose.cells.pivot/pivottable/column_range) | Restituisce un oggetto CellArea che rappresenta l'intervallo<br/> che contiene l'area della colonna nel rapporto di tabella pivot.|
| [row_range](/cells/it/python-net/aspose.cells.pivot/pivottable/row_range) | Restituisce un oggetto CellArea che rappresenta l'intervallo<br/> che contiene l'area della riga nel rapporto di tabella pivot.|
| [data_body_range](/cells/it/python-net/aspose.cells.pivot/pivottable/data_body_range) | Restituisce un oggetto CellArea che rappresenta l'intervallo che contiene l'area dati<br/> nell'elenco tra la riga di intestazione e la riga di inserimento.|
| [table_range1](/cells/it/python-net/aspose.cells.pivot/pivottable/table_range1) | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero rapporto di tabella pivot,<br/> ma non include i campi della pagina.|
| [table_range2](/cells/it/python-net/aspose.cells.pivot/pivottable/table_range2) | Restituisce un oggetto CellArea che rappresenta l'intervallo contenente l'intero rapporto di tabella pivot,<br/> include i campi della pagina.|
| [column_grand](/cells/it/python-net/aspose.cells.pivot/pivottable/column_grand) | Indica se il rapporto di tabella pivot mostra i totali complessivi per le colonne.|
| [is_grid_drop_zones](/cells/it/python-net/aspose.cells.pivot/pivottable/is_grid_drop_zones) | Indica se il rapporto di tabella pivot visualizza il layout di tabella pivot classico.<br/> (consente di trascinare i campi nella griglia)|
| [row_grand](/cells/it/python-net/aspose.cells.pivot/pivottable/row_grand) |Indica se il rapporto di tabella pivot mostra i totali complessivi per le righe.|
| [display_null_string](/cells/it/python-net/aspose.cells.pivot/pivottable/display_null_string) | Indica se il rapporto di tabella pivot visualizza una stringa personalizzata<br/> nelle celle che contengono valori nulli.|
| [null_string](/cells/it/python-net/aspose.cells.pivot/pivottable/null_string) | Ottiene la stringa visualizzata nelle celle che contengono valori Null<br/> quando la proprietà DisplayNullString è true.|
| [display_error_string](/cells/it/python-net/aspose.cells.pivot/pivottable/display_error_string) | Indica se il rapporto di tabella pivot visualizza una stringa personalizzata nelle celle che contengono errori.|
| [data_field_header_name](/cells/it/python-net/aspose.cells.pivot/pivottable/data_field_header_name) | Ottiene e imposta il nome dell'intestazione del campo dell'area del valore nella tabella pivot.|
| [error_string](/cells/it/python-net/aspose.cells.pivot/pivottable/error_string) | Ottiene la stringa visualizzata nelle celle che contengono errori<br/> quando la proprietà DisplayErrorString è true.Il valore predefinito è una stringa vuota.|
| [is_auto_format](/cells/it/python-net/aspose.cells.pivot/pivottable/is_auto_format) | Indica se il rapporto di tabella pivot viene formattato automaticamente.<br/>Casella di controllo "tabella di formattazione automatica" che si trova nell'opzione pivottable per Excel 2003<br/> Casella di controllo "adatta automaticamente la larghezza della colonna all'aggiornamento" che si trova nella tabella pivot Opzioni: Formato layout per Excel 2007|
| [auto_format_type](/cells/it/python-net/aspose.cells.pivot/pivottable/auto_format_type) | Ottiene il tipo di formato automatico della tabella pivot.|
| [has_blank_rows](/cells/it/python-net/aspose.cells.pivot/pivottable/has_blank_rows) | Indica se aggiungere righe vuote.<br/>Questa proprietà si applica solo ai tipi di formato automatico della tabella pivot che devono aggiungere righe vuote.|
| [merge_labels](/cells/it/python-net/aspose.cells.pivot/pivottable/merge_labels) | Indica se l'elemento della riga esterna, l'elemento della colonna, il totale parziale,<br/> e le etichette del totale complessivo utilizzano celle unite.|
| [preserve_formatting](/cells/it/python-net/aspose.cells.pivot/pivottable/preserve_formatting) | Indica se la formattazione viene mantenuta quando la tabella pivot viene aggiornata o ricalcolata.|
| [show_drill](/cells/it/python-net/aspose.cells.pivot/pivottable/show_drill) | Ottiene se vengono visualizzati i pulsanti di espansione/compressione.|
| [enable_drilldown](/cells/it/python-net/aspose.cells.pivot/pivottable/enable_drilldown) | Ottiene se il drill-down è abilitato.|
| [enable_field_dialog](/cells/it/python-net/aspose.cells.pivot/pivottable/enable_field_dialog) | Indica se la finestra di dialogo Campo tabella pivot è disponibile<br/> quando l'utente fa doppio clic sul campo della tabella pivot.|
| [enable_field_list](/cells/it/python-net/aspose.cells.pivot/pivottable/enable_field_list) | Ottiene se abilitare l'elenco dei campi per la tabella pivot.|
| [enable_wizard](/cells/it/python-net/aspose.cells.pivot/pivottable/enable_wizard) | Indica se la Creazione guidata tabella pivot è disponibile.|
| [subtotal_hidden_page_items](/cells/it/python-net/aspose.cells.pivot/pivottable/subtotal_hidden_page_items) | Indica se gli elementi del campo della pagina nascosti nel rapporto di tabella pivot<br/>sono inclusi nei subtotali di riga e colonna, nei totali di blocco e nei totali complessivi.<br/> Il valore predefinito è falso.|
| [grand_total_name](/cells/it/python-net/aspose.cells.pivot/pivottable/grand_total_name) | Restituisce l'etichetta della stringa di testo visualizzata nell'intestazione di riga o colonna del totale complessivo.<br/> Il valore predefinito è la stringa "Grand Total".|
| [manual_update](/cells/it/python-net/aspose.cells.pivot/pivottable/manual_update) |Indica se il rapporto di tabella pivot viene ricalcolato solo su richiesta dell'utente.|
| [is_multiple_field_filters](/cells/it/python-net/aspose.cells.pivot/pivottable/is_multiple_field_filters) | Specifica un valore booleano che indica se i campi di una tabella pivot possono avere più filtri impostati su di essi.|
| [missing_items_limit](/cells/it/python-net/aspose.cells.pivot/pivottable/missing_items_limit) | Specifica un valore booleano che indica se i campi di una tabella pivot possono avere più filtri impostati su di essi.|
| [enable_data_value_editing](/cells/it/python-net/aspose.cells.pivot/pivottable/enable_data_value_editing) | Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della tabella pivot.<br/> Abilita la modifica delle celle nell'area dei valori|
| [show_data_tips](/cells/it/python-net/aspose.cells.pivot/pivottable/show_data_tips) | Specifica un valore booleano che indica se le descrizioni comandi devono essere visualizzate per le celle di dati della tabella pivot.|
| [show_member_property_tips](/cells/it/python-net/aspose.cells.pivot/pivottable/show_member_property_tips) | Specifica un valore booleano che indica se le informazioni sulla proprietà del membro devono essere omesse dalle descrizioni comando della tabella pivot.|
| [show_values_row](/cells/it/python-net/aspose.cells.pivot/pivottable/show_values_row) | Specifica un valore booleano che indica se visualizzare la riga dei valori.<br/> mostra la riga dei valori|
| [show_empty_col](/cells/it/python-net/aspose.cells.pivot/pivottable/show_empty_col) | Specifica un valore booleano che indica se includere colonne vuote nella tabella|
| [show_empty_row](/cells/it/python-net/aspose.cells.pivot/pivottable/show_empty_row) | Specifica un valore booleano che indica se includere righe vuote nella tabella.|
| [field_list_sort_ascending](/cells/it/python-net/aspose.cells.pivot/pivottable/field_list_sort_ascending) |Specifica un valore booleano che indica se i campi nella tabella pivot sono ordinati in un ordine non predefinito nell'elenco dei campi.|
| [print_drill](/cells/it/python-net/aspose.cells.pivot/pivottable/print_drill) | Specifica un valore booleano che indica se gli indicatori di drill devono essere stampati.<br/> stampa i pulsanti espandi/comprimi quando vengono visualizzati nella tabella pivot.|
| [alt_text_title](/cells/it/python-net/aspose.cells.pivot/pivottable/alt_text_title) | Ottiene il titolo dell'altertext|
| [alt_text_description](/cells/it/python-net/aspose.cells.pivot/pivottable/alt_text_description) | Ottiene la descrizione del testo alternativo|
| [name](/cells/it/python-net/aspose.cells.pivot/pivottable/name) | Ottiene il nome della tabella pivot|
| [column_header_caption](/cells/it/python-net/aspose.cells.pivot/pivottable/column_header_caption) | Ottiene la didascalia dell'intestazione di colonna della tabella pivot.|
| [indent](/cells/it/python-net/aspose.cells.pivot/pivottable/indent) | Specifica l'incremento di rientro per l'asse compatto e può essere utilizzato per impostare il layout del report su Forma compatta.|
| [row_header_caption](/cells/it/python-net/aspose.cells.pivot/pivottable/row_header_caption) | Ottiene la didascalia dell'intestazione di riga della tabella pivot.|
| [show_row_header_caption](/cells/it/python-net/aspose.cells.pivot/pivottable/show_row_header_caption) | Indica se la didascalia dell'intestazione di riga viene visualizzata nel rapporto di tabella pivot<br/> Indica se visualizzare le didascalie dei campi e gli elenchi a discesa dei filtri|
| [custom_list_sort](/cells/it/python-net/aspose.cells.pivot/pivottable/custom_list_sort) | Indica se considerare l'elenco personalizzato integrato durante l'ordinamento dei dati|
| [pivot_format_conditions](/cells/it/python-net/aspose.cells.pivot/pivottable/pivot_format_conditions) | Ottiene le condizioni di formato della tabella pivot.|
| [page_field_order](/cells/it/python-net/aspose.cells.pivot/pivottable/page_field_order) | Ottiene l'ordine in cui i campi della pagina vengono aggiunti al layout del rapporto di tabella pivot.|
| [page_field_wrap_count](/cells/it/python-net/aspose.cells.pivot/pivottable/page_field_wrap_count) |Ottiene il numero di campi pagina in ogni colonna o riga nel rapporto di tabella pivot.|
| [tag](/cells/it/python-net/aspose.cells.pivot/pivottable/tag) | Ottiene una stringa salvata con il rapporto di tabella pivot.|
| [save_data](/cells/it/python-net/aspose.cells.pivot/pivottable/save_data) | Indica se i dati per il rapporto di tabella pivot vengono salvati con la cartella di lavoro.|
| [refresh_data_on_opening_file](/cells/it/python-net/aspose.cells.pivot/pivottable/refresh_data_on_opening_file) | Indica se aggiornare i dati all'apertura del file.|
| [refresh_data_flag](/cells/it/python-net/aspose.cells.pivot/pivottable/refresh_data_flag) | Indica se aggiornare i dati o meno.|
| [external_connection_data_source](/cells/it/python-net/aspose.cells.pivot/pivottable/external_connection_data_source) | Ottiene l'origine dati della connessione esterna.|
| [data_source](/cells/it/python-net/aspose.cells.pivot/pivottable/data_source) | Ottiene e imposta l'origine dati della tabella pivot.|
| [item_print_titles](/cells/it/python-net/aspose.cells.pivot/pivottable/item_print_titles) | Bit che specifica se eseguire il pivot delle didascalie degli elementi sull'asse delle righe<br/> vengono ripetuti su ogni pagina stampata per i campi pivot in forma tabellare.|
| [print_titles](/cells/it/python-net/aspose.cells.pivot/pivottable/print_titles) | Indica se i titoli di stampa per il foglio di lavoro sono basati su set<br/> nel rapporto di tabella pivot.|
| [display_immediate_items](/cells/it/python-net/aspose.cells.pivot/pivottable/display_immediate_items) | Indica se gli elementi nelle aree di riga e colonna sono visibili<br/> quando l'area dati della tabella pivot è vuota.|
| [is_selected](/cells/it/python-net/aspose.cells.pivot/pivottable/is_selected) | Indica se la tabella pivot è selezionata.|
| [show_pivot_style_row_header](/cells/it/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_header) | Indica se lo stile deve essere applicato all'intestazione di riga nella tabella pivot.|
| [show_pivot_style_column_header](/cells/it/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_header) |Indica se lo stile deve essere applicato all'intestazione di colonna nella tabella pivot.|
| [show_pivot_style_row_stripes](/cells/it/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_stripes) | Indica se viene applicata la formattazione delle strisce di riga.|
| [show_pivot_style_column_stripes](/cells/it/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_stripes) | Indica se viene applicata la formattazione delle strisce di colonne.|
| [show_pivot_style_last_column](/cells/it/python-net/aspose.cells.pivot/pivottable/show_pivot_style_last_column) | Indica se viene applicata la formattazione delle strisce di colonne.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [remove_field(field_type, field_name)](/cells/it/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-str) | Rimuove un campo da un'area del campo specifica|
| [remove_field(field_type, base_field_index)](/cells/it/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-int) | Rimuove un campo da un'area del campo specifica|
| [remove_field(field_type, pivot_field)](/cells/it/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-PivotField) | Rimuovi campo da un'area di campo specifica|
| [add_field_to_area(field_type, field_name)](/cells/it/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-str) | Aggiunge il campo all'area specifica.|
| [add_field_to_area(field_type, base_field_index)](/cells/it/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-int) | Aggiunge il campo all'area specifica.|
| [add_field_to_area(field_type, pivot_field)](/cells/it/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-PivotField) | Aggiunge il campo all'area specifica.|
| [add_calculated_field(name, formula, drag_to_data_area)](/cells/it/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str-bool) | Aggiunge un campo calcolato al campo pivot.|
| [add_calculated_field(name, formula)](/cells/it/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str) | Aggiunge un campo calcolato al campo pivot e lo trascina nell'area dati.|
| [move(row, column)](/cells/it/python-net/aspose.cells.pivot/pivottable/move/#int-int) | Sposta la tabella pivot in una posizione diversa nel foglio di lavoro.|
| [move(dest_cell_name)](/cells/it/python-net/aspose.cells.pivot/pivottable/move/#str) | Sposta la tabella pivot in una posizione diversa nel foglio di lavoro.|
| [set_auto_group_field(base_field_index)](/cells/it/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#int) | Imposta il gruppo di campi automatico in base alla tabella pivot.|
| [set_auto_group_field(pivot_field)](/cells/it/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#PivotField) | Imposta il gruppo di campi automatico in base alla tabella pivot.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/it/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-float-float-list-float) | Imposta i gruppi di campi manuali in base alla tabella pivot.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/it/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-float-float-list-float) | Imposta i gruppi di campi manuali in base alla tabella pivot.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/it/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-DateTime-DateTime-list-int) | Imposta i gruppi di campi manuali in base alla tabella pivot.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/it/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-DateTime-DateTime-list-int) | Imposta i gruppi di campi manuali in base alla tabella pivot.|
| [set_ungroup(base_field_index)](/cells/it/python-net/aspose.cells.pivot/pivottable/set_ungroup/#int) | Gli insiemi separano in base alla tabella pivot|
| [set_ungroup(pivot_field)](/cells/it/python-net/aspose.cells.pivot/pivottable/set_ungroup/#PivotField) | Gli insiemi separano in base alla tabella pivot|
| [copy_style(pivot_table)](/cells/it/python-net/aspose.cells.pivot/pivottable/copy_style/#PivotTable) | Copia lo stile denominato da un'altra tabella pivot.|
| [show_report_filter_page(page_field)](/cells/it/python-net/aspose.cells.pivot/pivottable/show_report_filter_page/#PivotField) | Mostra tutte le pagine del filtro del report in base a PivotField, il PivotField deve trovarsi nei PageField.|
| [show_report_filter_page_by_name(field_name)](/cells/it/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_name/#str) | Mostra tutte le pagine del filtro del report in base al nome del PivotField, il PivotField deve trovarsi nei PageField.|
| [show_report_filter_page_by_index(pos_index)](/cells/it/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_index/#int) |Mostra tutte le pagine del filtro del report in base all'indice di posizione nei PageField|
| [fields(field_type)](/cells/it/python-net/aspose.cells.pivot/pivottable/fields/#PivotFieldType) | Ottiene i campi specifici in base al tipo di campo.|
| [change_data_source(source)](/cells/it/python-net/aspose.cells.pivot/pivottable/change_data_source/#list) | Imposta i dati di origine di pivottable.<br/> Foglio1!$A$1:$C$3|
| [get_source()](/cells/it/python-net/aspose.cells.pivot/pivottable/get_source/#) | Ottieni i dati di origine di pivottable.|
| [refresh_data()](/cells/it/python-net/aspose.cells.pivot/pivottable/refresh_data/#) | Aggiorna i dati e le impostazioni di pivottable dalla sua origine dati.|
| [calculate_data()](/cells/it/python-net/aspose.cells.pivot/pivottable/calculate_data/#) | Calcola i dati della tabella pivot in celle.|
| [clear_data()](/cells/it/python-net/aspose.cells.pivot/pivottable/clear_data/#) | Cancella i dati e la formattazione della tabella pivot|
| [calculate_range()](/cells/it/python-net/aspose.cells.pivot/pivottable/calculate_range/#) | Calcola l'intervallo di pivottable.|
| [format_all(style)](/cells/it/python-net/aspose.cells.pivot/pivottable/format_all/#Style) | Formatta tutte le celle nell'area della tabella pivot|
| [format_row(row, style)](/cells/it/python-net/aspose.cells.pivot/pivottable/format_row/#int-Style) | Formatta i dati della riga nell'area della tabella pivot|
| [format(row, column, style)](/cells/it/python-net/aspose.cells.pivot/pivottable/format/#int-int-Style) | Formatta la cella nell'area della tabella pivot|
| [get_horizontal_breaks()](/cells/it/python-net/aspose.cells.pivot/pivottable/get_horizontal_breaks/#) | ottieni l'elenco dell'indice delle righe della tabella pivot delle interruzioni di pagina orizzontali|
| [show_in_compact_form()](/cells/it/python-net/aspose.cells.pivot/pivottable/show_in_compact_form/#) | Dispone la tabella pivot in formato compatto.|
| [show_in_outline_form()](/cells/it/python-net/aspose.cells.pivot/pivottable/show_in_outline_form/#) | Dispone la tabella pivot sotto forma di struttura.|
| [show_in_tabular_form()](/cells/it/python-net/aspose.cells.pivot/pivottable/show_in_tabular_form/#) | Dispone la tabella pivot in formato tabulare.|
| [get_cell_by_display_name(display_name)](/cells/it/python-net/aspose.cells.pivot/pivottable/get_cell_by_display_name/#str) | Ottiene l'oggetto Cell in base al DisplayName di PivotField|
| [get_children()](/cells/it/python-net/aspose.cells.pivot/pivottable/get_children/#) | Ottiene le tabelle pivot figlio che utilizzano i dati della tabella pivot come origine dati.|



###  Esempi

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Guarda anche
* modulo [aspose.cells.pivot](..)
