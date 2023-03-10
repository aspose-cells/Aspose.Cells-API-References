---
title: classe PivotField
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 10
url: /it/python-net/aspose.cells.pivot/pivotfield/
is_root: false
---
##  classe PivotField
Rappresenta un campo in un rapporto di tabella pivot.



Il tipo PivotField espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [pivot_items](/cells/it/python-net/aspose.cells.pivot/pivotfield/pivot_items) | Ottiene gli elementi pivot del campo pivot|
| [range](/cells/it/python-net/aspose.cells.pivot/pivotfield/range) | Ottiene l'intervallo di gruppo del campo pivot|
| [is_calculated_field](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_calculated_field) | Indica se il campo della tabella pivot specificato è un campo calcolato.|
| [base_index](/cells/it/python-net/aspose.cells.pivot/pivotfield/base_index) | Rappresenta l'indice PivotField nei PivotField di base.|
| [position](/cells/it/python-net/aspose.cells.pivot/pivotfield/position) | Rappresenta l'indice PivotField nei PivotFields.|
| [name](/cells/it/python-net/aspose.cells.pivot/pivotfield/name) | Rappresenta il nome del campo pivot.|
| [display_name](/cells/it/python-net/aspose.cells.pivot/pivotfield/display_name) | Rappresenta il nome visualizzato di PivotField.|
| [is_auto_subtotals](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_auto_subtotals) | Indica se il campo specificato mostra totali parziali automatici. L'impostazione predefinita è true.|
| [drag_to_column](/cells/it/python-net/aspose.cells.pivot/pivotfield/drag_to_column) | Indica se il campo specificato può essere trascinato nella posizione della colonna.<br/> Il valore predefinito è vero.|
| [drag_to_hide](/cells/it/python-net/aspose.cells.pivot/pivotfield/drag_to_hide) | Indica se il campo specificato può essere trascinato nella posizione nascosta.<br/> Il valore predefinito è vero.|
| [drag_to_row](/cells/it/python-net/aspose.cells.pivot/pivotfield/drag_to_row) | Indica se il campo specificato può essere trascinato nella posizione della riga.<br/> Il valore predefinito è vero.|
| [drag_to_page](/cells/it/python-net/aspose.cells.pivot/pivotfield/drag_to_page) | Indica se il campo specificato può essere trascinato nella posizione della pagina.<br/> Il valore predefinito è vero.|
| [drag_to_data](/cells/it/python-net/aspose.cells.pivot/pivotfield/drag_to_data) |Indica se il campo specificato può essere trascinato nella posizione dei dati.<br/> Il valore predefinito è vero.|
| [is_multiple_item_selection_allowed](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_multiple_item_selection_allowed) | indica se il campo può avere più elementi<br/>selezionato nel campo della pagina<br/> Il valore predefinito è falso.|
| [is_repeat_item_labels](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_repeat_item_labels) | indica se il campo può ripetere le etichette degli elementi<br/> Il valore predefinito è falso.|
| [is_include_new_items_in_filter](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_include_new_items_in_filter) | indica se il campo può includere nuovi elementi nel filtro manuale<br/> Il valore predefinito è falso.|
| [is_insert_page_breaks_between_items](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_insert_page_breaks_between_items) | indica se il campo può inserire interruzioni di pagina tra gli elementi<br/>inserire un'interruzione di pagina dopo ogni elemento<br/> Il valore predefinito è falso.|
| [show_all_items](/cells/it/python-net/aspose.cells.pivot/pivotfield/show_all_items) | Indica se vengono visualizzati tutti gli elementi nel rapporto di tabella pivot,<br/>anche se non contengono dati di sintesi.<br/>mostra elementi senza dati<br/> Il valore predefinito è falso.|
| [non_auto_sort_default](/cells/it/python-net/aspose.cells.pivot/pivotfield/non_auto_sort_default) | Indica se un'operazione di ordinamento che verrà applicata a questo campo pivot è un'operazione di ordinamento automatico o un semplice ordinamento dei dati.|
| [is_auto_sort](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_auto_sort) | Indica se il campo della tabella pivot specificato viene ordinato automaticamente.|
| [is_ascend_sort](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_ascend_sort) | Indica se il campo della tabella pivot specificato è ordinato automaticamente in ordine crescente.|
| [auto_sort_field](/cells/it/python-net/aspose.cells.pivot/pivotfield/auto_sort_field) | Rappresenta l'indice del campo di ordinamento automatico.<br/> -1 indica PivotField stesso, altri indica la posizione dei campi dati.|
| [is_auto_show](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_auto_show) | Indica se il campo della tabella pivot specificato viene visualizzato automaticamente, valido solo per excel 2003.|
| [is_ascend_show](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_ascend_show) | Indica se il campo della tabella pivot specificato viene visualizzato automaticamente in ordine crescente.|
| [auto_show_count](/cells/it/python-net/aspose.cells.pivot/pivotfield/auto_show_count) |Rappresenta il numero di elementi superiori o inferiori<br/> che vengono mostrati automaticamente nel campo della tabella pivot specificato.|
| [auto_show_field](/cells/it/python-net/aspose.cells.pivot/pivotfield/auto_show_field) | Rappresenta l'indice del campo di visualizzazione automatica. -1 significa PivotField stesso.<br/> Dovrebbe essere l'indice dei campi dati.|
| [function](/cells/it/python-net/aspose.cells.pivot/pivotfield/function) | Rappresenta la funzione utilizzata per riepilogare il campo dati della tabella pivot.|
| [data_display_format](/cells/it/python-net/aspose.cells.pivot/pivotfield/data_display_format) | Rappresenta come visualizzare i valori contenuti in un campo dati.|
| [base_field_index](/cells/it/python-net/aspose.cells.pivot/pivotfield/base_field_index) | Rappresenta il campo base per un calcolo personalizzato.|
| [base_item_position](/cells/it/python-net/aspose.cells.pivot/pivotfield/base_item_position) | Rappresenta l'elemento nel campo base per un calcolo personalizzato.<br/> Valido solo per i campi dati.<br/>Poiché PivotItemPosition.Custom è solo per la lettura, se è necessario impostare PivotItemPosition.Custom,<br/> impostare l'attributo PivotField.BaseItemIndex.|
| [base_item_index](/cells/it/python-net/aspose.cells.pivot/pivotfield/base_item_index) | Rappresenta l'elemento nel campo base per un calcolo personalizzato.<br/> Valido solo per i campi dati.|
| [current_page_item](/cells/it/python-net/aspose.cells.pivot/pivotfield/current_page_item) | Rappresenta l'elemento della pagina corrente visualizzato per il campo pagina (valido solo per i campi pagina).|
| [number](/cells/it/python-net/aspose.cells.pivot/pivotfield/number) | Rappresenta il formato di visualizzazione predefinito di numeri e date.|
| [insert_blank_row](/cells/it/python-net/aspose.cells.pivot/pivotfield/insert_blank_row) | Indica se inserire una riga vuota dopo ogni elemento.|
| [show_subtotal_at_top](/cells/it/python-net/aspose.cells.pivot/pivotfield/show_subtotal_at_top) | quando ShowInOutlineForm è vero, visualizza i subtotali in cima all'elenco di elementi invece che in fondo|
| [show_in_outline_form](/cells/it/python-net/aspose.cells.pivot/pivotfield/show_in_outline_form) | Indica se il layout di questo campo è strutturato nella vista Tabella pivot|
| [number_format](/cells/it/python-net/aspose.cells.pivot/pivotfield/number_format) |Rappresenta il formato di visualizzazione personalizzato di numeri e date.|
| [items](/cells/it/python-net/aspose.cells.pivot/pivotfield/items) | Ottieni tutti gli oggetti di base;|
| [original_items](/cells/it/python-net/aspose.cells.pivot/pivotfield/original_items) | Ottieni gli oggetti di base originali;|
| [item_count](/cells/it/python-net/aspose.cells.pivot/pivotfield/item_count) | Ottiene il numero di elementi di base di questo campo pivot.|
| [show_compact](/cells/it/python-net/aspose.cells.pivot/pivotfield/show_compact) | Indica se visualizzare le etichette del campo successivo nella stessa colonna nella vista Tabella pivot|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [hide_item(index, is_hidden)](/cells/it/python-net/aspose.cells.pivot/pivotfield/hide_item/#int-bool) | Imposta se il PivotItem specifico in un campo dati è nascosto.|
| [hide_item(item_value, is_hidden)](/cells/it/python-net/aspose.cells.pivot/pivotfield/hide_item/#str-bool) | Imposta se il PivotItem specifico in un campo dati è nascosto.|
| [get_pivot_filter_by_type(type)](/cells/it/python-net/aspose.cells.pivot/pivotfield/get_pivot_filter_by_type/#PivotFilterType) | Ottiene il filtro pivot del campo pivot per tipo|
| [get_pivot_filters()](/cells/it/python-net/aspose.cells.pivot/pivotfield/get_pivot_filters/#) | Ottiene i filtri pivot del campo pivot|
| [init_pivot_items()](/cells/it/python-net/aspose.cells.pivot/pivotfield/init_pivot_items/#) | Inizializza gli elementi pivot del campo pivot|
| [get_calculated_field_formula()](/cells/it/python-net/aspose.cells.pivot/pivotfield/get_calculated_field_formula/#) | Ottenere la stringa della formula del campo calcolato specificato.|
| [set_subtotals(subtotal_type, shown)](/cells/it/python-net/aspose.cells.pivot/pivotfield/set_subtotals/#PivotFieldSubtotalType-bool) | Imposta se il campo specificato mostra i subtotali.|
| [get_subtotals(subtotal_type)](/cells/it/python-net/aspose.cells.pivot/pivotfield/get_subtotals/#PivotFieldSubtotalType) | Ottiene se il campo specificato mostra i subtotali.|
| [is_hidden_item(index)](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_hidden_item/#int) | Indica se il PivotItem specifico è nascosto.|
| [is_hidden_item_detail(index)](/cells/it/python-net/aspose.cells.pivot/pivotfield/is_hidden_item_detail/#int) | Indica se il PivotItem specifico è un dettaglio nascosto.|
| [hide_item_detail(index, is_hidden_detail)](/cells/it/python-net/aspose.cells.pivot/pivotfield/hide_item_detail/#int-bool) | Imposta se il PivotItem specifico in un campo pivot è un dettaglio nascosto.|
| [hide_detail(is_hidden_detail)](/cells/it/python-net/aspose.cells.pivot/pivotfield/hide_detail/#bool) | Imposta se i PivotItems in un campo pivot sono dettagli nascosti. Questo è comprimere/espandere questo campo.|
| [add_calculated_item(name, formula)](/cells/it/python-net/aspose.cells.pivot/pivotfield/add_calculated_item/#str-str) |Aggiungi un elemento calcolato al campo pivot.|



###  Esempio

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType

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
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Guarda anche
* modulo [aspose.cells.pivot](..)
