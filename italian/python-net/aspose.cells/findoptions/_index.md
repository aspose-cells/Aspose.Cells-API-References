---
title: classe FindOptions
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 630
url: /it/python-net/aspose.cells/findoptions/
is_root: false
---
##  classe FindOptions
Rappresenta le opzioni di ricerca.



Il tipo FindOptions espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [FindOptions()](/cells/it/python-net/aspose.cells/findoptions/__init__/#) | Costruisce una nuova istanza di FindOptions|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [is_case_sensitive](/cells/it/python-net/aspose.cells/findoptions/is_case_sensitive) | Indica se la stringa cercata fa distinzione tra maiuscole e minuscole.|
| [case_sensitive](/cells/it/python-net/aspose.cells/findoptions/case_sensitive) | Indica se la stringa cercata fa distinzione tra maiuscole e minuscole.|
| [look_at_type](/cells/it/python-net/aspose.cells/findoptions/look_at_type) | Guarda tipo.|
| [is_range_set](/cells/it/python-net/aspose.cells/findoptions/is_range_set) | Indica se l'intervallo di ricerca è impostato.|
| [search_next](/cells/it/python-net/aspose.cells/findoptions/search_next) | Ordine di ricerca. Vero: cerca dopo. Falso: ricerca precedente.|
| [search_backward](/cells/it/python-net/aspose.cells/findoptions/search_backward) | Indica se cercare all'indietro le celle.|
| [seach_order_by_rows](/cells/it/python-net/aspose.cells/findoptions/seach_order_by_rows) | Indica se l'ordine di ricerca è per righe o colonne.|
| [look_in_type](/cells/it/python-net/aspose.cells/findoptions/look_in_type) | Cerca nel tipo.|
| [regex_key](/cells/it/python-net/aspose.cells/findoptions/regex_key) | Indica se la chiave cercata è regex.<br/> Se vero, la chiave cercata verrà considerata come regex e analizzata. Altrimenti la chiave verrà analizzata secondo le regole in ms excel.|
| [value_type_sensitive](/cells/it/python-net/aspose.cells/findoptions/value_type_sensitive) | Indica se il tipo di valore della cella cercata deve essere uguale alla chiave cercata.|
| [style](/cells/it/python-net/aspose.cells/findoptions/style) | Il formato da cercare.|
| [convert_numeric_data](/cells/it/python-net/aspose.cells/findoptions/convert_numeric_data) | Ottiene o imposta un valore che indica se convertire il valore di stringa cercato in dati numerici.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [get_range()](/cells/it/python-net/aspose.cells/findoptions/get_range/#) | Ottiene e imposta l'intervallo cercato.|
| [set_range(ca)](/cells/it/python-net/aspose.cells/findoptions/set_range/#CellArea) | Imposta l'intervallo di ricerca.|



###  Esempio

```python
from aspose.cells import CellArea, FindOptions, LookInType, Workbook

# Instantiate the workbook object
workbook = Workbook("book1.xls")
# Get Cells collection
cells = workbook.worksheets[0].cells
# Instantiate FindOptions Object
findOptions = FindOptions()
# Create a Cells Area
ca = CellArea()
ca.start_row = 8
ca.start_column = 2
ca.end_row = 17
ca.end_column = 13
# Set cells area for find options
findOptions.set_range(ca)
# Set searching properties
findOptions.search_backward = False
findOptions.seach_order_by_rows = True
findOptions.look_in_type = LookInType.VALUES
# Find the cell with 0 value
cell = cells.find(0, None, findOptions)

```

###  Guarda anche
* modulo [aspose.cells](..)
