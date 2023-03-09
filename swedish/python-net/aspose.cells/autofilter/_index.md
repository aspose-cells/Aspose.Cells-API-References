---
title: AutoFilter klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 70
url: /sv/python-net/aspose.cells/autofilter/
is_root: false
---
##  AutoFilter klass
Representerar autofiltrering för det angivna kalkylbladet.



Typen AutoFilter avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [sorter](/cells/sv/python-net/aspose.cells/autofilter/sorter) | Hämtar datasorteraren.|
| [range](/cells/sv/python-net/aspose.cells/autofilter/range) | Representerar intervallet som det angivna autofiltret gäller.|
| [show_filter_button](/cells/sv/python-net/aspose.cells/autofilter/show_filter_button) | Indikerar om AutoFilter-knappen för denna kolumn är synlig.|
| [filter_columns](/cells/sv/python-net/aspose.cells/autofilter/filter_columns) | Hämtar samlingen av filterkolumnerna.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/sv/python-net/aspose.cells/autofilter/remove_filter/#int-str) |Tar bort ett filter för en filterkolumn.|
| [remove_filter(field_index)](/cells/sv/python-net/aspose.cells/autofilter/remove_filter/#int) | Ta bort det specifika filtret.|
| [custom(field_index, operator_type1, criteria1)](/cells/sv/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) | Filtrerar en lista med anpassade kriterier.|
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/sv/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) | Filtrerar en lista med anpassade kriterier.|
| [refresh()](/cells/sv/python-net/aspose.cells/autofilter/refresh/#) | Uppdatera automatiska filter för att dölja eller visa raderna.|
| [refresh(hide_rows)](/cells/sv/python-net/aspose.cells/autofilter/refresh/#bool) | Hämtar alla dolda raders index.|
| [set_range(row, start_column, end_column)](/cells/sv/python-net/aspose.cells/autofilter/set_range/#int-int-int) | Ställer in intervallet som det angivna autofiltret gäller för.|
| [get_cell_area()](/cells/sv/python-net/aspose.cells/autofilter/get_cell_area/#) | Hämtar [CellArea](/cells/sv/python-net/aspose.cells/cellarea) där det angivna autofiltret gäller.|
| [add_filter(field_index, criteria)](/cells/sv/python-net/aspose.cells/autofilter/add_filter/#int-str) | Lägger till ett filter för en filterkolumn.|
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/sv/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Lägger till ett datumfilter.|
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/sv/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Tar bort ett datumfilter.|
| [filter(field_index, criteria)](/cells/sv/python-net/aspose.cells/autofilter/filter/#int-str) | Filtrerar en lista med angivna kriterier.|
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/sv/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | Filtrera de 10 bästa objekten i listan|
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/sv/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) | Lägger till ett dynamiskt filter.|
| [add_font_color_filter(field_index, color)](/cells/sv/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) | Lägger till ett teckensnittsfärgfilter.|
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/sv/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) | Lägger till ett fyllningsfärgfilter.|
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/sv/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) | Lägger till ett ikonfilter.|
| [match_blanks(field_index)](/cells/sv/python-net/aspose.cells/autofilter/match_blanks/#int) | Matcha alla tomma celler i listan.|
| [match_non_blanks(field_index)](/cells/sv/python-net/aspose.cells/autofilter/match_non_blanks/#int) | Matcha alla inte tomma celler i listan.|
| [show_all()](/cells/sv/python-net/aspose.cells/autofilter/show_all/#) | Visa alla rader.|



###  Exempel

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

###  Se även
* modul [aspose.cells](..)
* klass [CellArea](/cells/sv/python-net/aspose.cells/cellarea)
