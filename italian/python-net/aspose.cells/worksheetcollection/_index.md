---
title: classe WorksheetCollection
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1630
url: /it/python-net/aspose.cells/worksheetcollection/
is_root: false
---
##  classe WorksheetCollection
Incapsula una raccolta di oggetti [Worksheet](/cells/it/python-net/aspose.cells/worksheet).



Il tipo WorksheetCollection espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [web_extension_task_panes](/cells/it/python-net/aspose.cells/worksheetcollection/web_extension_task_panes) | Ottiene l'elenco dei riquadri attività.|
| [web_extensions](/cells/it/python-net/aspose.cells/worksheetcollection/web_extensions) | Ottiene l'elenco dei riquadri attività.|
| [threaded_comment_authors](/cells/it/python-net/aspose.cells/worksheetcollection/threaded_comment_authors) | Ottiene l'elenco degli autori dei commenti con thread.|
| [is_refresh_all_connections](/cells/it/python-net/aspose.cells/worksheetcollection/is_refresh_all_connections) | Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel.|
| [names](/cells/it/python-net/aspose.cells/worksheetcollection/names) | Ottiene la raccolta di tutti gli oggetti Name nel foglio di calcolo.|
| [active_sheet_name](/cells/it/python-net/aspose.cells/worksheetcollection/active_sheet_name) | Rappresenta il nome del foglio di lavoro attivo all'apertura del foglio di calcolo.|
| [active_sheet_index](/cells/it/python-net/aspose.cells/worksheetcollection/active_sheet_index) | Rappresenta l'indice del foglio di lavoro attivo all'apertura del foglio di calcolo.|
| [dxfs](/cells/it/python-net/aspose.cells/worksheetcollection/dxfs) | Ottiene i record di formattazione differenziale master.|
| [xml_maps](/cells/it/python-net/aspose.cells/worksheetcollection/xml_maps) | Ottiene e imposta i mapping XML nella cartella di lavoro.|
| [built_in_document_properties](/cells/it/python-net/aspose.cells/worksheetcollection/built_in_document_properties) | Restituisce una raccolta [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty) che rappresenta tutte le proprietà del documento predefinite del foglio di calcolo.|
| [custom_document_properties](/cells/it/python-net/aspose.cells/worksheetcollection/custom_document_properties) | Restituisce una raccolta [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty) che rappresenta tutte le proprietà del documento personalizzato del foglio di calcolo.|
| [ole_size](/cells/it/python-net/aspose.cells/worksheetcollection/ole_size) | Ottiene e imposta le dimensioni visualizzate quando il file della cartella di lavoro viene utilizzato come oggetto Ole.|
| [external_links](/cells/it/python-net/aspose.cells/worksheetcollection/external_links) | Rappresenta collegamenti esterni in una cartella di lavoro.|
| [table_styles](/cells/it/python-net/aspose.cells/worksheetcollection/table_styles) | Ottiene l'oggetto [WorksheetCollection.table_styles](/cells/it/python-net/aspose.cells/worksheetcollection#table_styles).|
| [revision_logs](/cells/it/python-net/aspose.cells/worksheetcollection/revision_logs) |Rappresenta i registri di revisione.|
| [capacity](/cells/it/python-net/aspose.cells/worksheetcollection/capacity) | Ottiene o imposta il numero di elementi che l'elenco di matrici può contenere.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [get(index)](/cells/it/python-net/aspose.cells/worksheetcollection/get/#int) |Aggiungi API for Python tramite .Net.poiché questo[indice int] non è supportato|
| [get(sheet_name)](/cells/it/python-net/aspose.cells/worksheetcollection/get/#str) | Aggiungi API for Python tramite .Net.poiché this[string sheetName] non è supportato|
| [add(type)](/cells/it/python-net/aspose.cells/worksheetcollection/add/#SheetType) | Aggiunge un foglio di lavoro alla raccolta.|
| [add()](/cells/it/python-net/aspose.cells/worksheetcollection/add/#) | Aggiunge un foglio di lavoro alla raccolta.|
| [add(sheet_name)](/cells/it/python-net/aspose.cells/worksheetcollection/add/#str) | Aggiunge un foglio di lavoro alla raccolta.|
| [register_add_in_function(add_in_file, function_name, lib)](/cells/it/python-net/aspose.cells/worksheetcollection/register_add_in_function/#str-str-bool) | Aggiunge la funzione addin nella cartella di lavoro|
| [register_add_in_function(id, function_name)](/cells/it/python-net/aspose.cells/worksheetcollection/register_add_in_function/#int-str) | Aggiunge la funzione addin nella cartella di lavoro|
| [add_copy(sheet_name)](/cells/it/python-net/aspose.cells/worksheetcollection/add_copy/#str) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente.|
| [add_copy(sheet_index)](/cells/it/python-net/aspose.cells/worksheetcollection/add_copy/#int) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente.|
| [get_range_by_name(range_name)](/cells/it/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str) | Ottiene l'oggetto Range in base al nome predefinito.|
| [get_range_by_name(range_name, current_sheet_index, include_table)](/cells/it/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str-int-bool) | Ottiene [Range](/cells/it/python-net/aspose.cells/range) in base al nome predefinito o al nome della tabella|
| [copy_to(array)](/cells/it/python-net/aspose.cells/worksheetcollection/copy_to/#list) | Copia l'intero elenco di matrici in un elenco di matrici unidimensionale compatibile, a partire dall'inizio dell'elenco di matrici di destinazione.|
| [copy_to(index, array, array_index, count)](/cells/it/python-net/aspose.cells/worksheetcollection/copy_to/#int-list-int-int) |Copia un intervallo di elementi dall'elenco di matrici a un elenco di matrici unidimensionale compatibile, a partire dall'indice specificato dell'elenco di matrici di destinazione.|
| [index_of(item, index)](/cells/it/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dall'indice specificato all'ultimo elemento.|
| [index_of(item, index, count)](/cells/it/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero della prima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che inizia dall'indice specificato e contiene il numero specificato di elementi.|
| [last_index_of(item)](/cells/it/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intero elenco di matrici.|
| [last_index_of(item, index)](/cells/it/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int) | Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che si estende dal primo elemento all'indice specificato.|
| [last_index_of(item, index, count)](/cells/it/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int-int) |Cerca l'oggetto specificato e restituisce l'indice in base zero dell'ultima occorrenza all'interno dell'intervallo di elementi nell'elenco di matrici che contiene il numero specificato di elementi e termina con l'indice specificato.|
| [create_range(address, sheet_index)](/cells/it/python-net/aspose.cells/worksheetcollection/create_range/#str-int) | Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da un indirizzo dell'intervallo.|
| [create_union_range(address, sheet_index)](/cells/it/python-net/aspose.cells/worksheetcollection/create_union_range/#str-int) | Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da un indirizzo dell'intervallo.|
| [get_sheet_by_code_name(code_name)](/cells/it/python-net/aspose.cells/worksheetcollection/get_sheet_by_code_name/#str) | Ottiene il foglio di lavoro in base al nome in codice.|
| [sort_names()](/cells/it/python-net/aspose.cells/worksheetcollection/sort_names/#) | Ordina i nomi definiti.|
| [swap_sheet(sheet_index1, sheet_index2)](/cells/it/python-net/aspose.cells/worksheetcollection/swap_sheet/#int-int) | Scambia i due fogli.|
| [remove_at(name)](/cells/it/python-net/aspose.cells/worksheetcollection/remove_at/#str) | Rimuove l'elemento con un nome specificato.|
| [get_named_ranges()](/cells/it/python-net/aspose.cells/worksheetcollection/get_named_ranges/#) | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo.|
| [get_named_ranges_and_tables()](/cells/it/python-net/aspose.cells/worksheetcollection/get_named_ranges_and_tables/#) | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo.|
| [set_ole_size(start_row, end_row, start_column, end_column)](/cells/it/python-net/aspose.cells/worksheetcollection/set_ole_size/#int-int-int-int) | Imposta le dimensioni visualizzate quando il file della cartella di lavoro viene utilizzato come oggetto Ole.|
| [clear_pivottables()](/cells/it/python-net/aspose.cells/worksheetcollection/clear_pivottables/#) | Cancella le tabelle pivot dal foglio di calcolo.|
| [refresh_pivot_tables()](/cells/it/python-net/aspose.cells/worksheetcollection/refresh_pivot_tables/#) | Aggiorna tutte le tabelle pivot in WorksheetCollection.|
| [binary_search(item)](/cells/it/python-net/aspose.cells/worksheetcollection/binary_search/#Worksheet) | Cerca un elemento nell'intero elenco di matrici ordinate utilizzando l'operatore di confronto predefinito e restituisce l'indice in base zero dell'elemento.|



###  Esempi

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

###  Guarda anche
* modulo [aspose.cells](..)
* classe [DocumentProperty](/cells/it/python-net/aspose.cells.properties/documentproperty)
* classe [Range](/cells/it/python-net/aspose.cells/range)
* classe [Worksheet](/cells/it/python-net/aspose.cells/worksheet)
