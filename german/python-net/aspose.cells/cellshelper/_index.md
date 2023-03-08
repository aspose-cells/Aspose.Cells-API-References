---
title: CellsHelper Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 230
url: /de/python-net/aspose.cells/cellshelper/
is_root: false
---
##  CellsHelper Klasse
Bietet Hilfsfunktionen.



Der Typ CellsHelper macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [significant_digits](/cells/de/python-net/aspose.cells/cellshelper/significant_digits) | Ruft die Anzahl signifikanter Stellen ab und legt sie fest.<br/> Der Standardwert ist 17.|
| [dpi](/cells/de/python-net/aspose.cells/cellshelper/dpi) | Ruft die DPI des Computers ab.|
| [startup_path](/cells/de/python-net/aspose.cells/cellshelper/startup_path) | Ruft den Startpfad ab, auf den von einigen externen Formelverweisen verwiesen wird, oder legt diesen fest.|
| [alt_start_path](/cells/de/python-net/aspose.cells/cellshelper/alt_start_path) | Ruft den alternativen Startpfad ab, auf den von einigen externen Formelverweisen verwiesen wird, oder legt diesen fest.|
| [library_path](/cells/de/python-net/aspose.cells/cellshelper/library_path) | Ruft den Bibliothekspfad ab, auf den von einigen externen Formelreferenzen verwiesen wird, oder legt ihn fest.|
| [custom_implementation_factory](/cells/de/python-net/aspose.cells/cellshelper/custom_implementation_factory) | Ruft die Factory zum Erstellen von Instanzen mit spezieller Implementierung ab oder legt diese fest.|
| [is_cloud_platform](/cells/de/python-net/aspose.cells/cellshelper/is_cloud_platform) | Bitte setzen Sie diese Eigenschaft auf True, wenn Sie auf einer Cloud-Plattform ausgeführt werden, z. B.: Azure, AWSLambda usw.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [create_safe_sheet_name(name_proposal)](/cells/de/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str) | Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen.<br/>Wenn der angegebene Blattname den Regeln des Excel-Blattnamens entspricht, geben Sie ihn zurück.<br/>Andernfalls wird die Zeichenfolge abgeschnitten, wenn die Länge das Limit überschreitet<br/> und ungültige Zeichen werden durch ' ' ersetzt, geben dann den neu erstellten Zeichenfolgenwert zurück.|
| [create_safe_sheet_name(name_proposal, replace_char)](/cells/de/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str-char) | Überprüft den angegebenen Blattnamen und erstellt bei Bedarf einen gültigen.<br/>Wenn der angegebene Blattname den Regeln des Excel-Blattnamens entspricht, geben Sie ihn zurück.<br/>Andernfalls wird die Zeichenfolge abgeschnitten, wenn die Länge das Limit überschreitet<br/> und ungültige Zeichen werden durch das angegebene Zeichen ersetzt und geben dann den neu erstellten Zeichenfolgenwert zurück.|
| [get_text_width(text, font, scaling)](/cells/de/python-net/aspose.cells/cellshelper/get_text_width/#str-Font-float) | Holen Sie sich die Breite des Textes in Punkteinheiten.|
| [get_version()](/cells/de/python-net/aspose.cells/cellshelper/get_version/#) | Holen Sie sich die Release-Version.|
| [cell_name_to_index(cell_name, row, column)](/cells/de/python-net/aspose.cells/cellshelper/cell_name_to_index/#str-any-any) | Ruft die Zeilen- und Spaltenindizes der Zelle gemäß ihrem Namen ab.|
| [cell_index_to_name(row, column)](/cells/de/python-net/aspose.cells/cellshelper/cell_index_to_name/#int-int) | Ruft den Zellennamen gemäß seinen Zeilen- und Spaltenindizes ab.|
| [column_index_to_name(column)](/cells/de/python-net/aspose.cells/cellshelper/column_index_to_name/#int) | Ruft den Spaltennamen gemäß dem Spaltenindex ab.|
| [column_name_to_index(column_name)](/cells/de/python-net/aspose.cells/cellshelper/column_name_to_index/#str) | Ruft den Spaltenindex gemäß dem Spaltennamen ab.|
| [row_index_to_name(row)](/cells/de/python-net/aspose.cells/cellshelper/row_index_to_name/#int) | Ruft den Zeilennamen gemäß dem Zeilenindex ab.|
| [row_name_to_index(row_name)](/cells/de/python-net/aspose.cells/cellshelper/row_name_to_index/#str) | Ruft den Zeilenindex gemäß dem Zeilennamen ab.|
| [convert_r1c1_formula_to_a1(r_1c1_formula, row, column)](/cells/de/python-net/aspose.cells/cellshelper/convert_r1c1_formula_to_a1/#str-int-int) | Wandelt die r1c1-Formel der Zelle in eine A1-Formel um.|
| [convert_a1_formula_to_r1c1(formula, row, column)](/cells/de/python-net/aspose.cells/cellshelper/convert_a1_formula_to_r1c1/#str-int-int) | Konvertiert die A1-Formel der Zelle in die r1c1-Formel.|
| [get_date_time_from_double(double_value, date1904)](/cells/de/python-net/aspose.cells/cellshelper/get_date_time_from_double/#float-bool) | Konvertieren Sie den Double-Wert in den Datumszeitwert.|
| [get_double_from_date_time(date_time, date1904)](/cells/de/python-net/aspose.cells/cellshelper/get_double_from_date_time/#DateTime-bool) | Konvertieren Sie die Datumszeit in den doppelten Wert.|
| [get_used_colors(workbook)](/cells/de/python-net/aspose.cells/cellshelper/get_used_colors/#Workbook) | Ruft alle verwendeten Farben in der Arbeitsmappe ab.|
| [add_add_in_function(function, min_count_of_parameters, max_count_of_parameters, paramers_type, function_value_type)](/cells/de/python-net/aspose.cells/cellshelper/add_add_in_function/#str-int-int-list-ParameterType) | Add-in-Funktion hinzufügen.|
| [merge_files(files, cached_file, dest_file)](/cells/de/python-net/aspose.cells/cellshelper/merge_files/#list-str-str) | Führt einige große XLS-Dateien zu einer XLS-Datei zusammen.|
| [init_for_dot_net_core()](/cells/de/python-net/aspose.cells/cellshelper/init_for_dot_net_core/#) |Führen Sie die Initialisierung für das .NetCore-Programm durch.<br/> Wir empfehlen Ihnen, diese Methode zuerst für alle .NetCore-Initialisierungen aufzurufen.<br/>Zum Beispiel:<br/>CellsHelper.InitForDotNetCore();<br/> Arbeitsmappe wb = neue Arbeitsmappe();|



###  Siehe auch
* Modul [aspose.cells](..)
