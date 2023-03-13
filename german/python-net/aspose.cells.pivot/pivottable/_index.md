---
title: PivotTable Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 100
url: /de/python-net/aspose.cells.pivot/pivottable/
is_root: false
---
##  PivotTable Klasse
Zusammenfassende Beschreibung für PivotTable.



Der Typ PivotTable macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [is_excel_2003_compatible](/cells/de/python-net/aspose.cells.pivot/pivottable/is_excel_2003_compatible) | Gibt an, ob die PivotTable beim Aktualisieren der PivotTable für Excel2003 kompatibel ist,<br/>wenn wahr, muss eine Zeichenfolge kleiner oder gleich 255 Zeichen sein, wenn die Zeichenfolge also größer als 255 Zeichen ist,<br/>es wird abgeschnitten. wenn falsch, hat eine Zeichenfolge die oben erwähnte Einschränkung nicht.<br/> Der Standardwert ist wahr.|
| [refreshed_by_who](/cells/de/python-net/aspose.cells.pivot/pivottable/refreshed_by_who) | Ruft den Namen des Benutzers ab, der die PivotTable zuletzt aktualisiert hat|
| [refresh_date](/cells/de/python-net/aspose.cells.pivot/pivottable/refresh_date) | Ruft das Datum ab, an dem die PivotTable zuletzt aktualisiert wurde.|
| [pivot_table_style_name](/cells/de/python-net/aspose.cells.pivot/pivottable/pivot_table_style_name) | Ruft den Namen des schwenkbaren Stils ab und legt ihn fest.|
| [pivot_table_style_type](/cells/de/python-net/aspose.cells.pivot/pivottable/pivot_table_style_type) | Ruft den integrierten Pivot-Tabellenstil ab und legt ihn fest.|
| [column_fields](/cells/de/python-net/aspose.cells.pivot/pivottable/column_fields) | Gibt ein PivotFields-Objekt zurück, das derzeit als Spaltenfelder angezeigt wird.|
| [row_fields](/cells/de/python-net/aspose.cells.pivot/pivottable/row_fields) | Gibt ein PivotFields-Objekt zurück, das derzeit als Zeilenfelder angezeigt wird.|
| [page_fields](/cells/de/python-net/aspose.cells.pivot/pivottable/page_fields) | Gibt ein PivotFields-Objekt zurück, das derzeit als Seitenfelder angezeigt wird.|
| [data_fields](/cells/de/python-net/aspose.cells.pivot/pivottable/data_fields) | Ruft ein PivotField-Objekt ab, das alle Datenfelder in einer PivotTable darstellt.<br/>Schreibgeschützt. Es wäre nur init, wenn zwei oder mehr Datenfelder in den DataPiovtFiels vorhanden sind.<br/>Es wird nur verwendet, um DataPivotField zum Zeilen-/Spaltenbereich der PivotTable hinzuzufügen. Standard ist im Zeilenbereich.|
| [data_field](/cells/de/python-net/aspose.cells.pivot/pivottable/data_field) | Ruft ein PivotField-Objekt ab, das alle Datenfelder in einer PivotTable darstellt.<br/>Schreibgeschützt. Es wäre nur init, wenn zwei oder mehr Datenfelder in den DataPiovtFiels vorhanden sind.<br/>Es wird nur verwendet, um DataPivotField zum Zeilen-/Spaltenbereich der PivotTable hinzuzufügen. Standard ist im Zeilenbereich.|
| [base_fields](/cells/de/python-net/aspose.cells.pivot/pivottable/base_fields) | Gibt ein PivotFields-Objekt zurück, das alle Felder im PivotTable-Bericht enthält|
| [pivot_filters](/cells/de/python-net/aspose.cells.pivot/pivottable/pivot_filters) | Gibt ein PivotFilterCollection-Objekt zurück.|
| [column_range](/cells/de/python-net/aspose.cells.pivot/pivottable/column_range) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt<br/> die den Spaltenbereich im PivotTable-Bericht enthält. Schreibgeschützt.|
| [row_range](/cells/de/python-net/aspose.cells.pivot/pivottable/row_range) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt<br/> die den Zeilenbereich im PivotTable-Bericht enthält. Schreibgeschützt.|
| [data_body_range](/cells/de/python-net/aspose.cells.pivot/pivottable/data_body_range) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Datenbereich enthält<br/> in der Liste zwischen der Kopfzeile und der Einfügezeile. Schreibgeschützt.|
| [table_range1](/cells/de/python-net/aspose.cells.pivot/pivottable/table_range1) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält.<br/> enthält jedoch keine Seitenfelder. Schreibgeschützt.|
| [table_range2](/cells/de/python-net/aspose.cells.pivot/pivottable/table_range2) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält.<br/> enthält Seitenfelder. Schreibgeschützt.|
| [column_grand](/cells/de/python-net/aspose.cells.pivot/pivottable/column_grand) | Gibt an, ob der PivotTable-Bericht Gesamtsummen für Spalten anzeigt.|
| [is_grid_drop_zones](/cells/de/python-net/aspose.cells.pivot/pivottable/is_grid_drop_zones) | Gibt an, ob der PivotTable-Bericht das klassische PivotTable-Layout anzeigt.<br/> (ermöglicht das Ziehen von Feldern im Raster)|
| [row_grand](/cells/de/python-net/aspose.cells.pivot/pivottable/row_grand) |Gibt an, ob der PivotTable-Bericht Gesamtsummen für Zeilen anzeigt.|
| [display_null_string](/cells/de/python-net/aspose.cells.pivot/pivottable/display_null_string) | Gibt an, ob der PivotTable-Bericht eine benutzerdefinierte Zeichenfolge anzeigt<br/> in Zellen, die Nullwerte enthalten.|
| [null_string](/cells/de/python-net/aspose.cells.pivot/pivottable/null_string) | Ruft die Zeichenfolge ab, die in Zellen angezeigt wird, die Nullwerte enthalten<br/> wenn die DisplayNullString-Eigenschaft wahr ist. Der Standardwert ist eine leere Zeichenfolge.|
| [display_error_string](/cells/de/python-net/aspose.cells.pivot/pivottable/display_error_string) | Gibt an, ob der PivotTable-Bericht eine benutzerdefinierte Zeichenfolge in Zellen anzeigt, die Fehler enthalten.|
| [data_field_header_name](/cells/de/python-net/aspose.cells.pivot/pivottable/data_field_header_name) | Ruft den Namen des Wertbereichsfeldheaders in der PivotTable ab und legt diesen fest.|
| [error_string](/cells/de/python-net/aspose.cells.pivot/pivottable/error_string) | Ruft die Zeichenfolge ab, die in Zellen angezeigt wird, die Fehler enthalten<br/> wenn die DisplayErrorString-Eigenschaft wahr ist. Der Standardwert ist eine leere Zeichenfolge.|
| [is_auto_format](/cells/de/python-net/aspose.cells.pivot/pivottable/is_auto_format) | Gibt an, ob der PivotTable-Bericht automatisch formatiert wird.<br/>Kontrollkästchen "Tabelle automatisch formatieren", das sich in der Pivottable-Option für Excel 2003 befindet<br/> Kontrollkästchen "Spaltenbreite bei Aktualisierung automatisch anpassen" in Pivot-Tabellenoptionen: Layoutformat für Excel 2007|
| [auto_format_type](/cells/de/python-net/aspose.cells.pivot/pivottable/auto_format_type) | Ruft den automatischen PivotTable-Formattyp ab.|
| [has_blank_rows](/cells/de/python-net/aspose.cells.pivot/pivottable/has_blank_rows) | Gibt an, ob leere Zeilen hinzugefügt werden sollen.<br/>Diese Eigenschaft gilt nur für die automatischen PivotTable-Formattypen, die leere Zeilen hinzufügen müssen.|
| [merge_labels](/cells/de/python-net/aspose.cells.pivot/pivottable/merge_labels) | Gibt an, ob das äußere Zeilenelement, das Spaltenelement, die Zwischensumme des angegebenen PivotTable-Berichts<br/> und Gesamtsummenbeschriftungen verwenden verbundene Zellen.|
| [preserve_formatting](/cells/de/python-net/aspose.cells.pivot/pivottable/preserve_formatting) | Gibt an, ob die Formatierung beibehalten wird, wenn die PivotTable aktualisiert oder neu berechnet wird.|
| [show_drill](/cells/de/python-net/aspose.cells.pivot/pivottable/show_drill) | Ruft ab, ob Schaltflächen zum Erweitern/Reduzieren angezeigt werden.|
| [enable_drilldown](/cells/de/python-net/aspose.cells.pivot/pivottable/enable_drilldown) | Ruft ab, ob Drilldown aktiviert ist.|
| [enable_field_dialog](/cells/de/python-net/aspose.cells.pivot/pivottable/enable_field_dialog) | Gibt an, ob das Dialogfeld PivotTable-Feld verfügbar ist<br/> wenn der Benutzer auf das PivotTable-Feld doppelklickt.|
| [enable_field_list](/cells/de/python-net/aspose.cells.pivot/pivottable/enable_field_list) | Ruft ab, ob die Feldliste für die PivotTable aktiviert ist.|
| [enable_wizard](/cells/de/python-net/aspose.cells.pivot/pivottable/enable_wizard) | Gibt an, ob der PivotTable-Assistent verfügbar ist.|
| [subtotal_hidden_page_items](/cells/de/python-net/aspose.cells.pivot/pivottable/subtotal_hidden_page_items) | Gibt an, ob Seitenfeldelemente im PivotTable-Bericht ausgeblendet sind<br/>sind in Zeilen- und Spaltenzwischensummen, Blocksummen und Gesamtsummen enthalten.<br/> Der Standardwert ist False.|
| [grand_total_name](/cells/de/python-net/aspose.cells.pivot/pivottable/grand_total_name) | Gibt die Beschriftung der Textzeichenfolge zurück, die in der Spalten- oder Zeilenüberschrift der Gesamtsumme angezeigt wird.<br/> Der Standardwert ist die Zeichenfolge "Gesamtsumme".|
| [manual_update](/cells/de/python-net/aspose.cells.pivot/pivottable/manual_update) |Gibt an, ob der PivotTable-Bericht nur auf Anforderung des Benutzers neu berechnet wird.|
| [is_multiple_field_filters](/cells/de/python-net/aspose.cells.pivot/pivottable/is_multiple_field_filters) | Gibt einen booleschen Wert an, der angibt, ob für die Felder einer PivotTable mehrere Filter festgelegt werden können.|
| [missing_items_limit](/cells/de/python-net/aspose.cells.pivot/pivottable/missing_items_limit) | Gibt einen booleschen Wert an, der angibt, ob für die Felder einer PivotTable mehrere Filter festgelegt werden können.|
| [enable_data_value_editing](/cells/de/python-net/aspose.cells.pivot/pivottable/enable_data_value_editing) | Gibt einen booleschen Wert an, der angibt, ob der Benutzer berechtigt ist, die Zellen im Datenbereich der PivotTable zu bearbeiten.<br/> Aktivieren Sie die Zellenbearbeitung im Wertebereich|
| [show_data_tips](/cells/de/python-net/aspose.cells.pivot/pivottable/show_data_tips) | Gibt einen booleschen Wert an, der angibt, ob QuickInfos für PivotTable-Datenzellen angezeigt werden sollen.|
| [show_member_property_tips](/cells/de/python-net/aspose.cells.pivot/pivottable/show_member_property_tips) | Gibt einen booleschen Wert an, der angibt, ob Informationen zu Elementeigenschaften in PivotTable-QuickInfos weggelassen werden sollen.|
| [show_values_row](/cells/de/python-net/aspose.cells.pivot/pivottable/show_values_row) | Gibt einen booleschen Wert an, der angibt, ob die Wertezeile angezeigt wird.<br/> Zeigen Sie die Wertezeile an|
| [show_empty_col](/cells/de/python-net/aspose.cells.pivot/pivottable/show_empty_col) | Gibt einen booleschen Wert an, der angibt, ob leere Spalten in die Tabelle aufgenommen werden sollen|
| [show_empty_row](/cells/de/python-net/aspose.cells.pivot/pivottable/show_empty_row) | Gibt einen booleschen Wert an, der angibt, ob leere Zeilen in die Tabelle aufgenommen werden sollen.|
| [field_list_sort_ascending](/cells/de/python-net/aspose.cells.pivot/pivottable/field_list_sort_ascending) |Gibt einen booleschen Wert an, der angibt, ob Felder in der PivotTable in der Feldliste in einer nicht standardmäßigen Reihenfolge sortiert sind.|
| [print_drill](/cells/de/python-net/aspose.cells.pivot/pivottable/print_drill) | Gibt einen booleschen Wert an, der angibt, ob Bohrindikatoren gedruckt werden sollen.<br/> Schaltflächen zum Erweitern/Reduzieren drucken, wenn sie auf Pivottable angezeigt werden.|
| [alt_text_title](/cells/de/python-net/aspose.cells.pivot/pivottable/alt_text_title) | Ruft den Titel des Altertexts ab|
| [alt_text_description](/cells/de/python-net/aspose.cells.pivot/pivottable/alt_text_description) | Ruft die Beschreibung des Alternativtexts ab|
| [name](/cells/de/python-net/aspose.cells.pivot/pivottable/name) | Ruft den Namen der PivotTable ab|
| [column_header_caption](/cells/de/python-net/aspose.cells.pivot/pivottable/column_header_caption) | Ruft die Spaltenüberschrift der PivotTable ab.|
| [indent](/cells/de/python-net/aspose.cells.pivot/pivottable/indent) | Gibt das Einzugsinkrement für die kompakte Achse an und kann verwendet werden, um das Berichtslayout auf kompakte Form einzustellen.|
| [row_header_caption](/cells/de/python-net/aspose.cells.pivot/pivottable/row_header_caption) | Ruft die Zeilenkopfzeile der PivotTable ab.|
| [show_row_header_caption](/cells/de/python-net/aspose.cells.pivot/pivottable/show_row_header_caption) | Gibt an, ob die Zeilenkopfzeile im PivotTable-Bericht angezeigt wird<br/> Gibt an, ob Feldbeschriftungen und Filter-Dropdowns angezeigt werden|
| [custom_list_sort](/cells/de/python-net/aspose.cells.pivot/pivottable/custom_list_sort) | Gibt an, ob beim Sortieren von Daten die integrierte benutzerdefinierte Liste berücksichtigt wird|
| [pivot_format_conditions](/cells/de/python-net/aspose.cells.pivot/pivottable/pivot_format_conditions) | Ruft die Formatbedingungen der Pivot-Tabelle ab.|
| [page_field_order](/cells/de/python-net/aspose.cells.pivot/pivottable/page_field_order) | Ruft die Reihenfolge ab, in der Seitenfelder dem Layout des PivotTable-Berichts hinzugefügt werden.|
| [page_field_wrap_count](/cells/de/python-net/aspose.cells.pivot/pivottable/page_field_wrap_count) |Ruft die Anzahl der Seitenfelder in jeder Spalte oder Zeile im PivotTable-Bericht ab.|
| [tag](/cells/de/python-net/aspose.cells.pivot/pivottable/tag) | Ruft eine mit dem PivotTable-Bericht gespeicherte Zeichenfolge ab.|
| [save_data](/cells/de/python-net/aspose.cells.pivot/pivottable/save_data) | Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden.|
| [refresh_data_on_opening_file](/cells/de/python-net/aspose.cells.pivot/pivottable/refresh_data_on_opening_file) | Gibt an, ob Daten beim Öffnen einer Datei aktualisiert werden.|
| [refresh_data_flag](/cells/de/python-net/aspose.cells.pivot/pivottable/refresh_data_flag) | Gibt an, ob Daten aktualisieren oder nicht.|
| [external_connection_data_source](/cells/de/python-net/aspose.cells.pivot/pivottable/external_connection_data_source) | Ruft die externe Verbindungsdatenquelle ab.|
| [data_source](/cells/de/python-net/aspose.cells.pivot/pivottable/data_source) | Ruft die Datenquelle der Pivot-Tabelle ab und legt sie fest.|
| [item_print_titles](/cells/de/python-net/aspose.cells.pivot/pivottable/item_print_titles) | Ein Bit, das angibt, ob Pivot-Elementbeschriftungen auf der Zeilenachse angezeigt werden<br/> werden auf jeder Druckseite für Pivot-Felder in tabellarischer Form wiederholt.|
| [print_titles](/cells/de/python-net/aspose.cells.pivot/pivottable/print_titles) | Gibt an, ob die Drucktitel für das Arbeitsblatt satzbasiert sind<br/> im PivotTable-Bericht. Der Standardwert ist falsch.|
| [display_immediate_items](/cells/de/python-net/aspose.cells.pivot/pivottable/display_immediate_items) | Gibt an, ob Elemente in den Zeilen- und Spaltenbereichen sichtbar sind<br/> wenn der Datenbereich der PivotTable leer ist. Der Standardwert ist wahr.|
| [is_selected](/cells/de/python-net/aspose.cells.pivot/pivottable/is_selected) | Gibt an, ob die PivotTable ausgewählt ist.|
| [show_pivot_style_row_header](/cells/de/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_header) | Gibt an, ob der Stil auf die Zeilenüberschrift in der Pivot-Tabelle angewendet werden soll.|
| [show_pivot_style_column_header](/cells/de/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_header) |Gibt an, ob der Stil auf die Spaltenüberschrift in der Pivot-Tabelle angewendet werden soll.|
| [show_pivot_style_row_stripes](/cells/de/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_stripes) | Gibt an, ob Zeilenstreifenformatierung angewendet wird.|
| [show_pivot_style_column_stripes](/cells/de/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_stripes) | Gibt an, ob Spaltenstreifenformatierung angewendet wird.|
| [show_pivot_style_last_column](/cells/de/python-net/aspose.cells.pivot/pivottable/show_pivot_style_last_column) | Gibt an, ob Spaltenstreifenformatierung angewendet wird.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [remove_field(field_type, field_name)](/cells/de/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-str) | Entfernt ein Feld aus einem bestimmten Feldbereich|
| [remove_field(field_type, base_field_index)](/cells/de/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-int) | Entfernt ein Feld aus einem bestimmten Feldbereich|
| [remove_field(field_type, pivot_field)](/cells/de/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-PivotField) | Feld aus einem bestimmten Feldbereich entfernen|
| [add_field_to_area(field_type, field_name)](/cells/de/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-str) | Fügt das Feld dem bestimmten Bereich hinzu.|
| [add_field_to_area(field_type, base_field_index)](/cells/de/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-int) | Fügt das Feld dem bestimmten Bereich hinzu.|
| [add_field_to_area(field_type, pivot_field)](/cells/de/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-PivotField) | Fügt das Feld dem bestimmten Bereich hinzu.|
| [add_calculated_field(name, formula, drag_to_data_area)](/cells/de/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str-bool) | Fügt dem Pivot-Feld ein berechnetes Feld hinzu.|
| [add_calculated_field(name, formula)](/cells/de/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str) | Fügt ein berechnetes Feld zum Pivot-Feld hinzu und zieht es in den Datenbereich.|
| [move(row, column)](/cells/de/python-net/aspose.cells.pivot/pivottable/move/#int-int) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt.|
| [move(dest_cell_name)](/cells/de/python-net/aspose.cells.pivot/pivottable/move/#str) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt.|
| [set_auto_group_field(base_field_index)](/cells/de/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#int) | Legt die automatische Feldgruppe durch die PivotTable fest.|
| [set_auto_group_field(pivot_field)](/cells/de/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#PivotField) | Legt die automatische Feldgruppe durch die PivotTable fest.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/de/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-float-float-list-float) | Legt die manuelle Feldgruppe durch die PivotTable fest.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/de/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-float-float-list-float) | Legt die manuelle Feldgruppe durch die PivotTable fest.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/de/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-DateTime-DateTime-list-int) | Legt die manuelle Feldgruppe durch die PivotTable fest.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/de/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-DateTime-DateTime-list-int) | Legt die manuelle Feldgruppe durch die PivotTable fest.|
| [set_ungroup(base_field_index)](/cells/de/python-net/aspose.cells.pivot/pivottable/set_ungroup/#int) | Legt die Gruppierung durch die PivotTable fest|
| [set_ungroup(pivot_field)](/cells/de/python-net/aspose.cells.pivot/pivottable/set_ungroup/#PivotField) | Legt die Gruppierung durch die PivotTable fest|
| [copy_style(pivot_table)](/cells/de/python-net/aspose.cells.pivot/pivottable/copy_style/#PivotTable) | Kopiert den benannten Stil aus einer anderen Pivot-Tabelle.|
| [show_report_filter_page(page_field)](/cells/de/python-net/aspose.cells.pivot/pivottable/show_report_filter_page/#PivotField) | Alle Berichtsfilterseiten nach PivotField anzeigen, das PivotField muss sich in den PageFields befinden.|
| [show_report_filter_page_by_name(field_name)](/cells/de/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_name/#str) | Zeigen Sie alle Berichtsfilterseiten gemäß dem Namen von PivotField an, das PivotField muss sich in den PageFields befinden.|
| [show_report_filter_page_by_index(pos_index)](/cells/de/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_index/#int) |Alle Berichtsfilterseiten gemäß dem Positionsindex in den PageFields anzeigen|
| [fields(field_type)](/cells/de/python-net/aspose.cells.pivot/pivottable/fields/#PivotFieldType) | Ruft die spezifischen Felder nach Feldtyp ab.|
| [change_data_source(source)](/cells/de/python-net/aspose.cells.pivot/pivottable/change_data_source/#list) | Legen Sie die Quelldaten von Pivottable fest.<br/> Blatt1!$A$1:$C$3|
| [get_source()](/cells/de/python-net/aspose.cells.pivot/pivottable/get_source/#) | Rufen Sie die Quelldaten von Pivottable ab.|
| [refresh_data()](/cells/de/python-net/aspose.cells.pivot/pivottable/refresh_data/#) | Aktualisiert die Daten und Einstellungen der Pivottable aus ihrer Datenquelle.|
| [calculate_data()](/cells/de/python-net/aspose.cells.pivot/pivottable/calculate_data/#) | Berechnet die Daten von Pivottables in Zellen.|
| [clear_data()](/cells/de/python-net/aspose.cells.pivot/pivottable/clear_data/#) | Löschen Sie die Daten und die Formatierung von PivotTable|
| [calculate_range()](/cells/de/python-net/aspose.cells.pivot/pivottable/calculate_range/#) | Berechnet die Reichweite von Pivottables.|
| [format_all(style)](/cells/de/python-net/aspose.cells.pivot/pivottable/format_all/#Style) | Formatieren Sie alle Zellen im schwenkbaren Bereich|
| [format_row(row, style)](/cells/de/python-net/aspose.cells.pivot/pivottable/format_row/#int-Style) | Formatieren Sie die Zeilendaten im schwenkbaren Bereich|
| [format(row, column, style)](/cells/de/python-net/aspose.cells.pivot/pivottable/format/#int-int-Style) | Formatieren Sie die Zelle im schwenkbaren Bereich|
| [get_horizontal_breaks()](/cells/de/python-net/aspose.cells.pivot/pivottable/get_horizontal_breaks/#) | Abrufen der Pivot-Tabellenzeilenindexliste der horizontalen Seitenumbrüche|
| [show_in_compact_form()](/cells/de/python-net/aspose.cells.pivot/pivottable/show_in_compact_form/#) | Layoutt die PivotTable in kompakter Form.|
| [show_in_outline_form()](/cells/de/python-net/aspose.cells.pivot/pivottable/show_in_outline_form/#) | Layouts der PivotTable in Gliederungsform.|
| [show_in_tabular_form()](/cells/de/python-net/aspose.cells.pivot/pivottable/show_in_tabular_form/#) | Layouts der PivotTable in tabellarischer Form.|
| [get_cell_by_display_name(display_name)](/cells/de/python-net/aspose.cells.pivot/pivottable/get_cell_by_display_name/#str) | Ruft das Cell-Objekt anhand des Anzeigenamens von PivotField ab|
| [get_children()](/cells/de/python-net/aspose.cells.pivot/pivottable/get_children/#) | Ruft die untergeordneten PivotTables ab, die diese PivotTable-Daten als Datenquelle verwenden.|



###  Beispiel

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Siehe auch
* Modul [aspose.cells.pivot](..)
