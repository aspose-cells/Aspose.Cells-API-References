---
title: AutoFilter Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 70
url: /de/python-net/aspose.cells/autofilter/
is_root: false
---
##  AutoFilter Klasse
Stellt die automatische Filterung für das angegebene Arbeitsblatt dar.



Der Typ AutoFilter macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [sorter](/cells/de/python-net/aspose.cells/autofilter/sorter) | Ruft den Datensortierer ab.|
| [range](/cells/de/python-net/aspose.cells/autofilter/range) | Stellt den Bereich dar, für den der angegebene AutoFilter gilt.|
| [show_filter_button](/cells/de/python-net/aspose.cells/autofilter/show_filter_button) | Gibt an, ob die AutoFilter-Schaltfläche für diese Spalte sichtbar ist.|
| [filter_columns](/cells/de/python-net/aspose.cells/autofilter/filter_columns) | Ruft die Auflistung der Filterspalten ab.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/de/python-net/aspose.cells/autofilter/remove_filter/#int-str) | Entfernt einen Filter für eine Filterspalte.|
| [remove_filter(field_index)](/cells/de/python-net/aspose.cells/autofilter/remove_filter/#int) | Entfernen Sie den spezifischen Filter.|
| [custom(field_index, operator_type1, criteria1)](/cells/de/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) | Filtert eine Liste mit benutzerdefinierten Kriterien.|
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/de/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) | Filtert eine Liste mit benutzerdefinierten Kriterien.|
| [refresh()](/cells/de/python-net/aspose.cells/autofilter/refresh/#) | Aktualisieren Sie die automatischen Filter, um die Zeilen auszublenden oder einzublenden.|
| [refresh(hide_rows)](/cells/de/python-net/aspose.cells/autofilter/refresh/#bool) | Ruft die Indizes aller versteckten Zeilen ab.|
| [set_range(row, start_column, end_column)](/cells/de/python-net/aspose.cells/autofilter/set_range/#int-int-int) | Legt den Bereich fest, auf den der angegebene AutoFilter angewendet wird.|
| [get_cell_area()](/cells/de/python-net/aspose.cells/autofilter/get_cell_area/#) | Ruft die [CellArea](/cells/de/python-net/aspose.cells/cellarea) ab, auf die der angegebene AutoFilter zutrifft.|
| [add_filter(field_index, criteria)](/cells/de/python-net/aspose.cells/autofilter/add_filter/#int-str) | Fügt einen Filter für eine Filterspalte hinzu.|
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/de/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Fügt einen Datumsfilter hinzu.|
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/de/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Entfernt einen Datumsfilter.|
| [filter(field_index, criteria)](/cells/de/python-net/aspose.cells/autofilter/filter/#int-str) |Filtert eine Liste mit angegebenen Kriterien.|
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/de/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | Filtern Sie die Top-10-Elemente in der Liste|
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/de/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) | Fügt einen dynamischen Filter hinzu.|
| [add_font_color_filter(field_index, color)](/cells/de/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) | Fügt einen Schriftfarbenfilter hinzu.|
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/de/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) | Fügt einen Füllfarbenfilter hinzu.|
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/de/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) | Fügt einen Symbolfilter hinzu.|
| [match_blanks(field_index)](/cells/de/python-net/aspose.cells/autofilter/match_blanks/#int) | Übereinstimmung mit allen leeren Zellen in der Liste.|
| [match_non_blanks(field_index)](/cells/de/python-net/aspose.cells/autofilter/match_non_blanks/#int) | Übereinstimmung mit allen nicht leeren Zellen in der Liste.|
| [show_all()](/cells/de/python-net/aspose.cells/autofilter/show_all/#) | Alle Zeilen einblenden.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [CellArea](/cells/de/python-net/aspose.cells/cellarea)
