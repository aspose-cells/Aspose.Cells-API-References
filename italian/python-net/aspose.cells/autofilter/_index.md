---
title: classe AutoFilter
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells/autofilter/
is_root: false
---
##  classe AutoFilter
Rappresenta il filtro automatico per il foglio di lavoro specificato.



Il tipo AutoFilter espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [sorter](/cells/it/python-net/aspose.cells/autofilter/sorter) | Ottiene l'ordinatore di dati.|
| [range](/cells/it/python-net/aspose.cells/autofilter/range) | Rappresenta l'intervallo a cui si applica il filtro automatico specificato.|
| [show_filter_button](/cells/it/python-net/aspose.cells/autofilter/show_filter_button) | Indica se il pulsante Filtro automatico per questa colonna è visibile.|
| [filter_columns](/cells/it/python-net/aspose.cells/autofilter/filter_columns) | Ottiene la raccolta delle colonne del filtro.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/it/python-net/aspose.cells/autofilter/remove_filter/#int-str) |Rimuove un filtro per una colonna filtro.|
| [remove_filter(field_index)](/cells/it/python-net/aspose.cells/autofilter/remove_filter/#int) | Rimuovere il filtro specifico.|
| [custom(field_index, operator_type1, criteria1)](/cells/it/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) | Filtra un elenco con criteri personalizzati.|
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/it/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) | Filtra un elenco con criteri personalizzati.|
| [refresh()](/cells/it/python-net/aspose.cells/autofilter/refresh/#) | Aggiorna i filtri automatici per nascondere o visualizzare le righe.|
| [refresh(hide_rows)](/cells/it/python-net/aspose.cells/autofilter/refresh/#bool) | Ottiene gli indici di tutte le righe nascoste.|
| [set_range(row, start_column, end_column)](/cells/it/python-net/aspose.cells/autofilter/set_range/#int-int-int) | Imposta l'intervallo a cui si applica il filtro automatico specificato.|
| [get_cell_area()](/cells/it/python-net/aspose.cells/autofilter/get_cell_area/#) | Ottiene [CellArea](/cells/it/python-net/aspose.cells/cellarea) a cui si applica il filtro automatico specificato.|
| [add_filter(field_index, criteria)](/cells/it/python-net/aspose.cells/autofilter/add_filter/#int-str) | Aggiunge un filtro per una colonna filtro.|
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/it/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Aggiunge un filtro data.|
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/it/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Rimuove un filtro data.|
| [filter(field_index, criteria)](/cells/it/python-net/aspose.cells/autofilter/filter/#int-str) | Filtra un elenco con i criteri specificati.|
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/it/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | Filtra i primi 10 elementi nell'elenco|
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/it/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) | Aggiunge un filtro dinamico.|
| [add_font_color_filter(field_index, color)](/cells/it/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) | Aggiunge un filtro per il colore del carattere.|
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/it/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) | Aggiunge un filtro colore di riempimento.|
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/it/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) | Aggiunge un filtro icona.|
| [match_blanks(field_index)](/cells/it/python-net/aspose.cells/autofilter/match_blanks/#int) | Corrisponde a tutte le celle vuote nell'elenco.|
| [match_non_blanks(field_index)](/cells/it/python-net/aspose.cells/autofilter/match_non_blanks/#int) | Abbina tutte le celle non vuote nell'elenco.|
| [show_all()](/cells/it/python-net/aspose.cells/autofilter/show_all/#) | Scopri tutte le righe.|



###  Esempio

```python
from aspose.cells import Workbook

# Creating a file stream containing the Excel file to be opened
# Instantiating a Workbook object
workbook = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating AutoFilter by giving the cells range of the heading row
worksheet.auto_filter.range = "A1:B1"
# Filtering columns with specified values
worksheet.auto_filter.filter(1, "Bananas")
# Saving the modified Excel file.
workbook.save("output.xls")

```

###  Guarda anche
* modulo [aspose.cells](..)
* classe [CellArea](/cells/it/python-net/aspose.cells/cellarea)
