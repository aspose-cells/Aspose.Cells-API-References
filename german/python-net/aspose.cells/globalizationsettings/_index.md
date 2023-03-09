---
title: GlobalizationSettings Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 730
url: /de/python-net/aspose.cells/globalizationsettings/
is_root: false
---
##  GlobalizationSettings Klasse
Stellt die Globalisierungseinstellungen dar.



Der Typ GlobalizationSettings macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [GlobalizationSettings()](/cells/de/python-net/aspose.cells/globalizationsettings/__init__/#) | Erstellt eine neue Instanz von GlobalizationSettings|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [chart_settings](/cells/de/python-net/aspose.cells/globalizationsettings/chart_settings) | Ruft die Globalisierungseinstellungen für Chart ab oder legt diese fest.|
| [pivot_settings](/cells/de/python-net/aspose.cells/globalizationsettings/pivot_settings) | Ruft die Globalisierungseinstellungen für die Pivot-Tabelle ab oder legt diese fest.|
| [list_separator](/cells/de/python-net/aspose.cells/globalizationsettings/list_separator) | Ruft das Trennzeichen für Liste, Funktionsparameter usw. ab.|
| [row_separator_of_formula_array](/cells/de/python-net/aspose.cells/globalizationsettings/row_separator_of_formula_array) | Ruft das Trennzeichen für Zeilen in Arraydaten in Formel ab.|
| [column_separator_of_formula_array](/cells/de/python-net/aspose.cells/globalizationsettings/column_separator_of_formula_array) | Ruft das Trennzeichen für die Elemente in den Zeilendaten des Arrays in der Formel ab.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [get_pivot_total_name()](/cells/de/python-net/aspose.cells/globalizationsettings/get_pivot_total_name/#) | Ruft den Namen der Bezeichnung „Gesamt“ in der PivotTable ab.<br/> Sie müssen diese Methode überschreiben, wenn die PivotTable zwei oder mehr PivotFields im Datenbereich enthält.|
| [get_pivot_grand_total_name()](/cells/de/python-net/aspose.cells/globalizationsettings/get_pivot_grand_total_name/#) | Ruft den Namen der Bezeichnung „Gesamtsumme“ in der PivotTable ab.|
| [get_multiple_items_name()](/cells/de/python-net/aspose.cells/globalizationsettings/get_multiple_items_name/#) | Ruft den Namen der Bezeichnung „(Mehrere Elemente)“ in der PivotTable ab.|
| [get_all_name()](/cells/de/python-net/aspose.cells/globalizationsettings/get_all_name/#) | Ruft den Namen der Bezeichnung „(Alle)“ in der PivotTable ab.|
| [get_protection_name_of_pivot_table()](/cells/de/python-net/aspose.cells/globalizationsettings/get_protection_name_of_pivot_table/#) |Ruft den Schutznamen in der PivotTable ab.|
| [get_column_labels_of_pivot_table()](/cells/de/python-net/aspose.cells/globalizationsettings/get_column_labels_of_pivot_table/#) | Ruft den Namen der Bezeichnung „Spaltenbeschriftungen“ in der PivotTable ab.|
| [get_row_labels_name_of_pivot_table()](/cells/de/python-net/aspose.cells/globalizationsettings/get_row_labels_name_of_pivot_table/#) | Ruft den Namen der Bezeichnung „Zeilenbeschriftungen“ in der PivotTable ab.|
| [get_empty_data_name()](/cells/de/python-net/aspose.cells/globalizationsettings/get_empty_data_name/#) | Ruft den Namen der Bezeichnung „(leer)“ in der PivotTable ab.|
| [get_data_field_header_name_of_pivot_table()](/cells/de/python-net/aspose.cells/globalizationsettings/get_data_field_header_name_of_pivot_table/#) | Ruft den Namen des Wertbereichsfeldheaders in der PivotTable ab.|
| [get_sub_total_name(sub_total_type)](/cells/de/python-net/aspose.cells/globalizationsettings/get_sub_total_name/#aspose.cells.pivot.PivotFieldSubtotalType) | Ruft den Namen des Typs [PivotFieldSubtotalType](/cells/de/python-net/aspose.cells.pivot/pivotfieldsubtotaltype) in der PivotTable ab.|
| [get_total_name(function_type)](/cells/de/python-net/aspose.cells/globalizationsettings/get_total_name/#ConsolidationFunction) | Ruft den Gesamtnamen der Funktion ab.|
| [get_grand_total_name(function_type)](/cells/de/python-net/aspose.cells/globalizationsettings/get_grand_total_name/#ConsolidationFunction) | Ruft den Gesamtsummennamen der Funktion ab.|
| [get_table_row_type_of_headers()](/cells/de/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_headers/#) | Ruft den Typnamen von Tabellenzeilen ab, der aus dem Tabellenkopf besteht.<br/> Standard ist "Headers", also repräsentiert "#Headers" in der Formel den Tabellenkopf.|
| [get_table_row_type_of_data()](/cells/de/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_data/#) | Ruft den Typnamen von Tabellenzeilen ab, die aus dem Datenbereich der referenzierten Tabelle bestehen.<br/> Standard ist "Data", also repräsentiert "#Data" in der Formel den Datenbereich der Tabelle.|
| [get_table_row_type_of_all()](/cells/de/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_all/#) | Ruft den Typnamen von Tabellenzeilen ab, die aus allen Zeilen in der referenzierten Tabelle bestehen.<br/>Der Standardwert ist „Alle“, sodass in der Formel „#Alle“ alle Zeilen in der referenzierten Tabelle darstellt.|
| [get_table_row_type_of_totals()](/cells/de/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_totals/#) | Ruft den Typnamen von Tabellenzeilen ab, die aus der Gesamtzeile der referenzierten Tabelle bestehen.<br/> Der Standardwert ist „Totals“, sodass in der Formel „#Totals“ die Gesamtzeile der referenzierten Tabelle darstellt.|
| [get_table_row_type_of_current()](/cells/de/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_current/#) | Ruft den Typnamen von Tabellenzeilen ab, die aus der aktuellen Zeile in der referenzierten Tabelle bestehen.<br/> Der Standardwert ist „Diese Zeile“, sodass in der Formel „#Diese Zeile“ die aktuelle Zeile in der referenzierten Tabelle darstellt.|
| [get_error_value_string(err)](/cells/de/python-net/aspose.cells/globalizationsettings/get_error_value_string/#str) | Ruft den Anzeigezeichenfolgenwert für den Fehlerwert der Zelle ab|
| [get_boolean_value_string(bv)](/cells/de/python-net/aspose.cells/globalizationsettings/get_boolean_value_string/#bool) | Ruft den Anzeigezeichenfolgenwert für den booleschen Wert der Zelle ab|
| [get_local_function_name(standard_name)](/cells/de/python-net/aspose.cells/globalizationsettings/get_local_function_name/#str) | Ruft den vom Gebietsschema abhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen ab.|
| [get_standard_function_name(local_name)](/cells/de/python-net/aspose.cells/globalizationsettings/get_standard_function_name/#str) | Ruft den Standardfunktionsnamen gemäß dem angegebenen gebietsschemaabhängigen Funktionsnamen ab.|
| [get_local_built_in_name(standard_name)](/cells/de/python-net/aspose.cells/globalizationsettings/get_local_built_in_name/#str) | Ruft den vom Gebietsschema abhängigen Text für den integrierten Namen gemäß dem angegebenen Standardtext ab.|
| [get_standard_built_in_name(local_name)](/cells/de/python-net/aspose.cells/globalizationsettings/get_standard_built_in_name/#str) | Ruft den Standardtext des integrierten Namens gemäß dem angegebenen gebietsschemaabhängigen Text ab.|
| [get_standard_header_footer_font_style_name(localfont_style_name)](/cells/de/python-net/aspose.cells/globalizationsettings/get_standard_header_footer_font_style_name/#str) |Ruft den standardmäßigen englischen Schriftstilnamen (regulär, fett, kursiv) für die Kopf-/Fußzeile gemäß dem angegebenen Gebietsschema-Schriftstilnamen ab.|
| [get_comment_title_name(type)](/cells/de/python-net/aspose.cells/globalizationsettings/get_comment_title_name/#aspose.cells.rendering.CommentTitleType) | Ruft den vom Gebietsschema abhängigen Kommentartitelnamen gemäß dem Kommentartiteltyp ab.|
| [compare(v1, v2, ignore_case)](/cells/de/python-net/aspose.cells/globalizationsettings/compare/#str-str-bool) | Vergleicht zwei Zeichenfolgenwerte gemäß bestimmten Sortierregeln.|



###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [PivotFieldSubtotalType](/cells/de/python-net/aspose.cells.pivot/pivotfieldsubtotaltype)
