---
title: ListObject Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells.tables/listobject/
is_root: false
---
##  ListObject Klasse
Stellt ein Listenobjekt auf einem Arbeitsblatt dar.
 Das Objekt ListObject ist ein Mitglied der ListObjects-Auflistung.
Die ListObjects-Auflistung enthält alle Listenobjekte auf einem Arbeitsblatt.



Der Typ ListObject macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [start_row](/cells/de/python-net/aspose.cells.tables/listobject/start_row) | Ruft die Startzeile des Bereichs ab.|
| [start_column](/cells/de/python-net/aspose.cells.tables/listobject/start_column) | Ruft die Startspalte des Bereichs ab.|
| [end_row](/cells/de/python-net/aspose.cells.tables/listobject/end_row) | Ruft die Endzeile des Bereichs ab.|
| [end_column](/cells/de/python-net/aspose.cells.tables/listobject/end_column) | Ruft die Endspalte des Bereichs ab.|
| [list_columns](/cells/de/python-net/aspose.cells.tables/listobject/list_columns) | Ruft ListColumns des ListObject ab.|
| [show_header_row](/cells/de/python-net/aspose.cells.tables/listobject/show_header_row) | Ruft ab und legt fest, ob dieses ListObject eine Kopfzeile anzeigt.|
| [show_totals](/cells/de/python-net/aspose.cells.tables/listobject/show_totals) |Ruft ab und legt fest, ob dieses ListObject die Gesamtzeile anzeigt.|
| [data_range](/cells/de/python-net/aspose.cells.tables/listobject/data_range) | Ruft den Datenbereich des ListObject ab.|
| [query_table](/cells/de/python-net/aspose.cells.tables/listobject/query_table) |Ruft die verknüpfte QueryTable ab.|
| [data_source_type](/cells/de/python-net/aspose.cells.tables/listobject/data_source_type) | Ruft den Datenquellentyp der Tabelle ab.|
| [auto_filter](/cells/de/python-net/aspose.cells.tables/listobject/auto_filter) | Ruft Autofilter ab.|
| [display_name](/cells/de/python-net/aspose.cells.tables/listobject/display_name) | Ruft den Anzeigenamen ab und legt ihn fest.|
| [comment](/cells/de/python-net/aspose.cells.tables/listobject/comment) | Ruft den Kommentar der Tabelle ab und legt ihn fest.|
| [show_table_style_first_column](/cells/de/python-net/aspose.cells.tables/listobject/show_table_style_first_column) | Gibt an, ob der Stil auf die erste Spalte in der Tabelle angewendet werden soll.|
| [show_table_style_last_column](/cells/de/python-net/aspose.cells.tables/listobject/show_table_style_last_column) | Gibt an, ob der Stil auf die letzte Spalte in der Tabelle angewendet werden soll.|
| [show_table_style_row_stripes](/cells/de/python-net/aspose.cells.tables/listobject/show_table_style_row_stripes) | Gibt an, ob Zeilenstreifenformatierung angewendet wird.|
| [show_table_style_column_stripes](/cells/de/python-net/aspose.cells.tables/listobject/show_table_style_column_stripes) | Gibt an, ob Spaltenstreifenformatierung angewendet wird.|
| [table_style_type](/cells/de/python-net/aspose.cells.tables/listobject/table_style_type) | Ruft und den integrierten Tabellenstil ab.|
| [table_style_name](/cells/de/python-net/aspose.cells.tables/listobject/table_style_name) | Ruft den Namen des Tabellenstils ab und legt ihn fest.|
| [xml_map](/cells/de/python-net/aspose.cells.tables/listobject/xml_map) | Ruft eine [ListObject.xml_map](/cells/de/python-net/aspose.cells.tables/listobject#xml_map) ab, die für diese Liste verwendet wird.|
| [alternative_text](/cells/de/python-net/aspose.cells.tables/listobject/alternative_text) | Ruft den alternativen Text ab und legt ihn fest.|
| [alternative_description](/cells/de/python-net/aspose.cells.tables/listobject/alternative_description) | Ruft die alternative Beschreibung ab und legt sie fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [convert_to_range()](/cells/de/python-net/aspose.cells.tables/listobject/convert_to_range/#) | Wandeln Sie die Tabelle in einen Bereich um.|
| [convert_to_range(options)](/cells/de/python-net/aspose.cells.tables/listobject/convert_to_range/#TableToRangeOptions) | Wandeln Sie die Tabelle in einen Bereich um.|
| [resize(start_row, start_column, end_row, end_column, has_headers)](/cells/de/python-net/aspose.cells.tables/listobject/resize/#int-int-int-int-bool) | Größe des Bereichs des Listenobjekts ändern.|
| [put_cell_value(row_offset, column_offset, value)](/cells/de/python-net/aspose.cells.tables/listobject/put_cell_value/#int-int-any) | Geben Sie den Wert in die Zelle ein.|
| [update_column_name()](/cells/de/python-net/aspose.cells.tables/listobject/update_column_name/#) |Aktualisiert den Namen aller Listenspalten aus dem Arbeitsblatt.|
| [filter()](/cells/de/python-net/aspose.cells.tables/listobject/filter/#) | Filtern Sie die Tabelle.|
| [apply_style_to_range()](/cells/de/python-net/aspose.cells.tables/listobject/apply_style_to_range/#) | Wenden Sie den Tabellenstil auf den Bereich an.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells.tables](..)
