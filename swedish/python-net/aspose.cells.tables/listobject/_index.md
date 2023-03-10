---
title: ListObject klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells.tables/listobject/
is_root: false
---
##  ListObject klass
Representerar ett listobjekt på ett kalkylblad.
 Objektet ListObject är en medlem av ListObjects-samlingen.
ListObjects-samlingen innehåller alla listobjekt på ett kalkylblad.



Typen ListObject avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [start_row](/cells/sv/python-net/aspose.cells.tables/listobject/start_row) | Hämtar intervallets startrad.|
| [start_column](/cells/sv/python-net/aspose.cells.tables/listobject/start_column) | Hämtar startkolumnen för intervallet.|
| [end_row](/cells/sv/python-net/aspose.cells.tables/listobject/end_row) | Hämtar den sista raden i intervallet.|
| [end_column](/cells/sv/python-net/aspose.cells.tables/listobject/end_column) |Hämtar slutkolumnen för intervallet.|
| [list_columns](/cells/sv/python-net/aspose.cells.tables/listobject/list_columns) | Hämtar ListColumns för ListObject.|
| [show_header_row](/cells/sv/python-net/aspose.cells.tables/listobject/show_header_row) | Hämtar och ställer in om detta ListObject visar rubrikrad.|
| [show_totals](/cells/sv/python-net/aspose.cells.tables/listobject/show_totals) | Hämtar och ställer in om detta ListObject visar total rad.|
| [data_range](/cells/sv/python-net/aspose.cells.tables/listobject/data_range) | Hämtar dataintervallet för ListObject.|
| [query_table](/cells/sv/python-net/aspose.cells.tables/listobject/query_table) | Hämtar den länkade frågetabellen.|
| [data_source_type](/cells/sv/python-net/aspose.cells.tables/listobject/data_source_type) | Hämtar datakällans typ för tabellen.|
| [auto_filter](/cells/sv/python-net/aspose.cells.tables/listobject/auto_filter) | Får autofilter.|
| [display_name](/cells/sv/python-net/aspose.cells.tables/listobject/display_name) | Hämtar och ställer in visningsnamnet.|
| [comment](/cells/sv/python-net/aspose.cells.tables/listobject/comment) | Får och ställer tabellens kommentar.|
| [show_table_style_first_column](/cells/sv/python-net/aspose.cells.tables/listobject/show_table_style_first_column) | Anger om den första kolumnen i tabellen ska ha stilen tillämpad.|
| [show_table_style_last_column](/cells/sv/python-net/aspose.cells.tables/listobject/show_table_style_last_column) | Anger om den sista kolumnen i tabellen ska ha stilen tillämpad.|
| [show_table_style_row_stripes](/cells/sv/python-net/aspose.cells.tables/listobject/show_table_style_row_stripes) | Indikerar om radrandsformatering tillämpas.|
| [show_table_style_column_stripes](/cells/sv/python-net/aspose.cells.tables/listobject/show_table_style_column_stripes) | Indikerar om formatering av kolumnrand används.|
| [table_style_type](/cells/sv/python-net/aspose.cells.tables/listobject/table_style_type) | Gets och den inbyggda bordsstilen.|
| [table_style_name](/cells/sv/python-net/aspose.cells.tables/listobject/table_style_name) | Hämtar och ställer in tabellstilens namn.|
| [xml_map](/cells/sv/python-net/aspose.cells.tables/listobject/xml_map) | Får ett [ListObject.xml_map](/cells/sv/python-net/aspose.cells.tables/listobject#xml_map) som används för denna lista.|
| [alternative_text](/cells/sv/python-net/aspose.cells.tables/listobject/alternative_text) | Hämtar och ställer in den alternativa texten.|
| [alternative_description](/cells/sv/python-net/aspose.cells.tables/listobject/alternative_description) | Hämtar och ställer in den alternativa beskrivningen.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [convert_to_range()](/cells/sv/python-net/aspose.cells.tables/listobject/convert_to_range/#) | Konvertera tabellen till intervall.|
| [convert_to_range(options)](/cells/sv/python-net/aspose.cells.tables/listobject/convert_to_range/#TableToRangeOptions) | Konvertera tabellen till intervall.|
| [resize(start_row, start_column, end_row, end_column, has_headers)](/cells/sv/python-net/aspose.cells.tables/listobject/resize/#int-int-int-int-bool) | Ändra storlek på intervallet för listobjektet.|
| [put_cell_value(row_offset, column_offset, value)](/cells/sv/python-net/aspose.cells.tables/listobject/put_cell_value/#int-int-any) | Lägg värdet i cellen.|
| [update_column_name()](/cells/sv/python-net/aspose.cells.tables/listobject/update_column_name/#) |Uppdaterar namnet på alla listkolumner från kalkylbladet.|
| [filter()](/cells/sv/python-net/aspose.cells.tables/listobject/filter/#) | Filtrera tabellen.|
| [apply_style_to_range()](/cells/sv/python-net/aspose.cells.tables/listobject/apply_style_to_range/#) | Tillämpa tabellstilen på intervallet.|



###  Exempel

```python
from aspose.cells import CellsHelper, Workbook
from aspose.cells.tables import TotalsCalculation

workbook = Workbook()
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(5):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_totals = True
table.list_columns[4].totals_calculation = TotalsCalculation.SUM
workbook.save(r"Book1.xlsx")

```

###  Se även
* modul [aspose.cells.tables](..)
