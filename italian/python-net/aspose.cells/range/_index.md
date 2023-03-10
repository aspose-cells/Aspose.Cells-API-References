---
title: classe Range
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1250
url: /it/python-net/aspose.cells/range/
is_root: false
---
##  classe Range
Incapsula l'oggetto che rappresenta un intervallo di celle all'interno di un foglio di calcolo.



Il tipo Range espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [current_region](/cells/it/python-net/aspose.cells/range/current_region) |Restituisce un oggetto Range che rappresenta l'area corrente.<br/> L'area corrente è un intervallo delimitato da qualsiasi combinazione di righe e colonne vuote.|
| [hyperlinks](/cells/it/python-net/aspose.cells/range/hyperlinks) | Ottiene tutti i collegamenti ipertestuali nell'intervallo.|
| [row_count](/cells/it/python-net/aspose.cells/range/row_count) | Ottiene il conteggio delle righe nell'intervallo.|
| [column_count](/cells/it/python-net/aspose.cells/range/column_count) | Ottiene il conteggio delle colonne nell'intervallo.|
| [cell_count](/cells/it/python-net/aspose.cells/range/cell_count) | Ottiene tutto il conteggio delle celle nell'intervallo.|
| [name](/cells/it/python-net/aspose.cells/range/name) | Ottiene o imposta il nome dell'intervallo.|
| [refers_to](/cells/it/python-net/aspose.cells/range/refers_to) | Ottiene i riferimenti dell'intervallo a.|
| [address](/cells/it/python-net/aspose.cells/range/address) | Ottiene l'indirizzo dell'intervallo.|
| [left](/cells/it/python-net/aspose.cells/range/left) | Ottiene la distanza, in punti, dal bordo sinistro della colonna A al bordo sinistro dell'intervallo.|
| [top](/cells/it/python-net/aspose.cells/range/top) | Ottiene la distanza, in punti, dal bordo superiore della riga 1 al bordo superiore dell'intervallo.|
| [width](/cells/it/python-net/aspose.cells/range/width) | Ottiene la larghezza di un intervallo in punti.|
| [height](/cells/it/python-net/aspose.cells/range/height) | Ottiene la larghezza di un intervallo in punti.|
| [first_row](/cells/it/python-net/aspose.cells/range/first_row) | Ottiene l'indice della prima riga dell'intervallo.|
| [first_column](/cells/it/python-net/aspose.cells/range/first_column) | Ottiene l'indice della prima colonna dell'intervallo.|
| [value](/cells/it/python-net/aspose.cells/range/value) | Ottiene e imposta il valore dell'intervallo.|
| [column_width](/cells/it/python-net/aspose.cells/range/column_width) | Imposta o ottiene la larghezza della colonna di questo intervallo|
| [row_height](/cells/it/python-net/aspose.cells/range/row_height) | Imposta o ottiene l'altezza delle righe in questo intervallo|
| [entire_column](/cells/it/python-net/aspose.cells/range/entire_column) |Ottiene un oggetto Range che rappresenta l'intera colonna (o le colonne) che contiene l'intervallo specificato.|
| [entire_row](/cells/it/python-net/aspose.cells/range/entire_row) | Ottiene un oggetto Range che rappresenta l'intera riga (o le righe) che contiene l'intervallo specificato.|
| [worksheet](/cells/it/python-net/aspose.cells/range/worksheet) | Ottiene l'oggetto [Range.worksheet](/cells/it/python-net/aspose.cells/range#worksheet) che contiene questo intervallo.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [auto_fill(target)](/cells/it/python-net/aspose.cells/range/auto_fill/#Range) | Riempiono automaticamente l'intervallo target.|
| [auto_fill(target, auto_fill_type)](/cells/it/python-net/aspose.cells/range/auto_fill/#Range-AutoFillType) | Riempiono automaticamente l'intervallo target.|
| [set_style(style, explicit_flag)](/cells/it/python-net/aspose.cells/range/set_style/#Style-bool) | Applicare lo stile della cella.|
| [set_style(style)](/cells/it/python-net/aspose.cells/range/set_style/#Style) | Imposta lo stile dell'intervallo.|
| [set_outline_borders(border_style, border_color)](/cells/it/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-CellsColor) | Imposta i bordi del contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo.|
| [set_outline_borders(border_style, border_color)](/cells/it/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-aspose.pydrawing.Color) | Imposta i bordi del contorno attorno a un intervallo di celle con lo stesso stile e colore del bordo.|
| [set_outline_borders(border_styles, border_colors)](/cells/it/python-net/aspose.cells/range/set_outline_borders/#list-aspose.pydrawing.Color[]) | Imposta i bordi della linea attorno a un intervallo di celle.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/it/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-CellsColor) | Imposta il bordo del contorno attorno a un intervallo di celle.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/it/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Imposta il bordo del contorno attorno a un intervallo di celle.|
| [copy(range, options)](/cells/it/python-net/aspose.cells/range/copy/#Range-PasteOptions) | Copia dell'intervallo con opzioni speciali di incolla.|
| [copy(range)](/cells/it/python-net/aspose.cells/range/copy/#Range) | Copia i dati (comprese le formule), la formattazione, gli oggetti di disegno ecc. da un intervallo di origine.|
| [get_enumerator()](/cells/it/python-net/aspose.cells/range/get_enumerator/#) | Ottiene l'enumeratore per le celle in questo Range.|
| [is_intersect(range)](/cells/it/python-net/aspose.cells/range/is_intersect/#Range) | Indica se l'intervallo è intersecato.|
| [intersect(range)](/cells/it/python-net/aspose.cells/range/intersect/#Range) | Restituisce un oggetto [Range](/cells/it/python-net/aspose.cells/range) che rappresenta l'intersezione rettangolare di due intervalli.|
| [union(range)](/cells/it/python-net/aspose.cells/range/union/#Range) | Restituisce l'unione di due intervalli.|
| [merge()](/cells/it/python-net/aspose.cells/range/merge/#) | Combina un intervallo di celle in una singola cella.|
| [un_merge()](/cells/it/python-net/aspose.cells/range/un_merge/#) |Separa le celle unite di questo intervallo.|
| [put_value(string_value, is_converted, set_style)](/cells/it/python-net/aspose.cells/range/put_value/#str-bool-bool) | Inserisce un valore nell'intervallo, se appropriato il valore verrà convertito in un altro tipo di dati e il formato numerico della cella verrà reimpostato.|
| [apply_style(style, flag)](/cells/it/python-net/aspose.cells/range/apply_style/#Style-StyleFlag) | Applica i formati per un'intera gamma.|
| [set_inside_borders(border_edge, line_style, border_color)](/cells/it/python-net/aspose.cells/range/set_inside_borders/#BorderType-CellBorderType-CellsColor) | Impostare all'interno dei bordi dell'intervallo.|
| [move_to(dest_row, dest_column)](/cells/it/python-net/aspose.cells/range/move_to/#int-int) | Sposta l'intervallo corrente nell'intervallo di destinazione.|
| [copy_data(range)](/cells/it/python-net/aspose.cells/range/copy_data/#Range) | Copia i dati della cella (comprese le formule) da un intervallo di origine.|
| [copy_value(range)](/cells/it/python-net/aspose.cells/range/copy_value/#Range) | Copia il valore della cella da un intervallo di origine.|
| [copy_style(range)](/cells/it/python-net/aspose.cells/range/copy_style/#Range) | Copia le impostazioni di stile da un intervallo di origine.|
| [get_cell_or_null(row_offset, column_offset)](/cells/it/python-net/aspose.cells/range/get_cell_or_null/#int-int) | Ottiene [Cell](/cells/it/python-net/aspose.cells/cell) oggetto o null in questo intervallo.|
| [get_offset(row_offset, column_offset)](/cells/it/python-net/aspose.cells/range/get_offset/#int-int) | Ottiene l'intervallo [Range](/cells/it/python-net/aspose.cells/range) in base all'offset.|



###  Esempio

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
#  Create a range (A1:D3).
range = cells.create_range("A1", "D3")
#  Set value to the range.
range.value = "Hello"
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [Cell](/cells/it/python-net/aspose.cells/cell)
* classe [Range](/cells/it/python-net/aspose.cells/range)
