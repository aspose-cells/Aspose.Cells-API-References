---
title: Range Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1250
url: /de/python-net/aspose.cells/range/
is_root: false
---
##  Range Klasse
Kapselt das Objekt, das einen Zellbereich in einer Tabelle darstellt.



Der Typ Range macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [current_region](/cells/de/python-net/aspose.cells/range/current_region) |Gibt ein Range-Objekt zurück, das die aktuelle Region darstellt.<br/> Der aktuelle Bereich ist ein Bereich, der durch eine beliebige Kombination aus leeren Zeilen und leeren Spalten begrenzt ist.|
| [hyperlinks](/cells/de/python-net/aspose.cells/range/hyperlinks) | Ruft alle Hyperlinks im Bereich ab.|
| [row_count](/cells/de/python-net/aspose.cells/range/row_count) | Ruft die Anzahl der Zeilen im Bereich ab.|
| [column_count](/cells/de/python-net/aspose.cells/range/column_count) | Ruft die Anzahl der Spalten im Bereich ab.|
| [cell_count](/cells/de/python-net/aspose.cells/range/cell_count) | Ruft alle Zellenzahlen im Bereich ab.|
| [name](/cells/de/python-net/aspose.cells/range/name) | Ruft den Namen des Bereichs ab oder legt diesen fest.|
| [refers_to](/cells/de/python-net/aspose.cells/range/refers_to) | Ruft die Verweise des Bereichs ab.|
| [address](/cells/de/python-net/aspose.cells/range/address) | Ruft die Adresse des Bereichs ab.|
| [left](/cells/de/python-net/aspose.cells/range/left) | Ruft den Abstand in Punkt vom linken Rand der Spalte A zum linken Rand des Bereichs ab.|
| [top](/cells/de/python-net/aspose.cells/range/top) | Ruft den Abstand in Punkt vom oberen Rand von Zeile 1 zum oberen Rand des Bereichs ab.|
| [width](/cells/de/python-net/aspose.cells/range/width) | Ruft die Breite eines Bereichs in Punkt ab.|
| [height](/cells/de/python-net/aspose.cells/range/height) | Ruft die Breite eines Bereichs in Punkt ab.|
| [first_row](/cells/de/python-net/aspose.cells/range/first_row) | Ruft den Index der ersten Zeile des Bereichs ab.|
| [first_column](/cells/de/python-net/aspose.cells/range/first_column) | Ruft den Index der ersten Spalte des Bereichs ab.|
| [value](/cells/de/python-net/aspose.cells/range/value) | Ruft den Wert des Bereichs ab und legt ihn fest.|
| [column_width](/cells/de/python-net/aspose.cells/range/column_width) | Legt die Spaltenbreite dieses Bereichs fest oder ruft sie ab|
| [row_height](/cells/de/python-net/aspose.cells/range/row_height) | Legt die Zeilenhöhe in diesem Bereich fest oder ruft sie ab|
| [entire_column](/cells/de/python-net/aspose.cells/range/entire_column) |Ruft ein Range-Objekt ab, das die gesamte Spalte (oder Spalten) darstellt, die den angegebenen Bereich enthält.|
| [entire_row](/cells/de/python-net/aspose.cells/range/entire_row) | Ruft ein Range-Objekt ab, das die gesamte Zeile (oder Zeilen) darstellt, die den angegebenen Bereich enthält.|
| [worksheet](/cells/de/python-net/aspose.cells/range/worksheet) | Ruft das [Range.worksheet](/cells/de/python-net/aspose.cells/range#worksheet)-Objekt ab, das diesen Bereich enthält.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [auto_fill(target)](/cells/de/python-net/aspose.cells/range/auto_fill/#Range) | Automatisch füllen alle den Zielbereich.|
| [auto_fill(target, auto_fill_type)](/cells/de/python-net/aspose.cells/range/auto_fill/#Range-AutoFillType) | Automatisch füllen alle den Zielbereich.|
| [set_style(style, explicit_flag)](/cells/de/python-net/aspose.cells/range/set_style/#Style-bool) | Wenden Sie den Zellenstil an.|
| [set_style(style)](/cells/de/python-net/aspose.cells/range/set_style/#Style) | Legt den Stil des Bereichs fest.|
| [set_outline_borders(border_style, border_color)](/cells/de/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-CellsColor) | Legt die Umrissrahmen um einen Bereich von Zellen mit demselben Rahmenstil und derselben Rahmenfarbe fest.|
| [set_outline_borders(border_style, border_color)](/cells/de/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-aspose.pydrawing.Color) | Legt die Umrissrahmen um einen Bereich von Zellen mit demselben Rahmenstil und derselben Rahmenfarbe fest.|
| [set_outline_borders(border_styles, border_colors)](/cells/de/python-net/aspose.cells/range/set_outline_borders/#list-aspose.pydrawing.Color[]) | Legt Linienränder um einen Bereich von Zellen fest.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/de/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-CellsColor) | Legt einen Umrissrahmen um einen Bereich von Zellen fest.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/de/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Legt einen Umrissrahmen um einen Bereich von Zellen fest.|
| [copy(range, options)](/cells/de/python-net/aspose.cells/range/copy/#Range-PasteOptions) | Kopieren des Bereichs mit speziellen Optionen zum Einfügen.|
| [copy(range)](/cells/de/python-net/aspose.cells/range/copy/#Range) | Kopiert Daten (einschließlich Formeln), Formatierungen, Zeichenobjekte usw. aus einem Quellbereich.|
| [get_enumerator()](/cells/de/python-net/aspose.cells/range/get_enumerator/#) | Ruft den Enumerator für Zellen in diesem Bereich ab.|
| [is_intersect(range)](/cells/de/python-net/aspose.cells/range/is_intersect/#Range) | Gibt an, ob sich der Bereich überschneidet.|
| [intersect(range)](/cells/de/python-net/aspose.cells/range/intersect/#Range) | Gibt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt zurück, das die rechteckige Schnittmenge zweier Bereiche darstellt.|
| [union(range)](/cells/de/python-net/aspose.cells/range/union/#Range) | Gibt die Vereinigung zweier Bereiche zurück.|
| [merge()](/cells/de/python-net/aspose.cells/range/merge/#) | Kombiniert eine Reihe von Zellen zu einer einzigen Zelle.|
| [un_merge()](/cells/de/python-net/aspose.cells/range/un_merge/#) |Hebt verbundene Zellen dieses Bereichs auf.|
| [put_value(string_value, is_converted, set_style)](/cells/de/python-net/aspose.cells/range/put_value/#str-bool-bool) | Fügt einen Wert in den Bereich ein, gegebenenfalls wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle wird zurückgesetzt.|
| [apply_style(style, flag)](/cells/de/python-net/aspose.cells/range/apply_style/#Style-StyleFlag) | Wendet Formate für eine ganze Reihe an.|
| [set_inside_borders(border_edge, line_style, border_color)](/cells/de/python-net/aspose.cells/range/set_inside_borders/#BorderType-CellBorderType-CellsColor) | Legen Sie innerhalb der Grenzen des Bereichs fest.|
| [move_to(dest_row, dest_column)](/cells/de/python-net/aspose.cells/range/move_to/#int-int) | Verschieben Sie den aktuellen Bereich in den Zielbereich.|
| [copy_data(range)](/cells/de/python-net/aspose.cells/range/copy_data/#Range) | Kopiert Zelldaten (einschließlich Formeln) aus einem Quellbereich.|
| [copy_value(range)](/cells/de/python-net/aspose.cells/range/copy_value/#Range) | Kopiert den Zellenwert aus einem Quellbereich.|
| [copy_style(range)](/cells/de/python-net/aspose.cells/range/copy_style/#Range) | Kopiert Stileinstellungen aus einem Quellbereich.|
| [get_cell_or_null(row_offset, column_offset)](/cells/de/python-net/aspose.cells/range/get_cell_or_null/#int-int) | Ruft [Cell](/cells/de/python-net/aspose.cells/cell) Objekt oder Null in diesem Bereich ab.|
| [get_offset(row_offset, column_offset)](/cells/de/python-net/aspose.cells/range/get_offset/#int-int) | Ruft den Bereich [Range](/cells/de/python-net/aspose.cells/range) nach Offset ab.|



###  Beispiele

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

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
* Klasse [Range](/cells/de/python-net/aspose.cells/range)
