---
title: Cell Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 140
url: /de/python-net/aspose.cells/cell/
is_root: false
---
##  Cell Klasse
Kapselt das Objekt, das eine einzelne Workbook-Zelle darstellt.



Der Typ Cell macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [worksheet](/cells/de/python-net/aspose.cells/cell/worksheet) | Ruft das übergeordnete Arbeitsblatt ab.|
| [date_time_value](/cells/de/python-net/aspose.cells/cell/date_time_value) | Ruft den in der Zelle enthaltenen DateTime-Wert ab.|
| [row](/cells/de/python-net/aspose.cells/cell/row) | Ruft die Zeilennummer (nullbasiert) der Zelle ab.|
| [column](/cells/de/python-net/aspose.cells/cell/column) | Ruft die Spaltennummer (nullbasiert) der Zelle ab.|
| [is_formula](/cells/de/python-net/aspose.cells/cell/is_formula) | Stellt dar, ob die angegebene Zelle eine Formel enthält.|
| [type](/cells/de/python-net/aspose.cells/cell/type) | Stellt den Zellwerttyp dar.|
| [name](/cells/de/python-net/aspose.cells/cell/name) | Ruft den Namen der Zelle ab.|
| [is_error_value](/cells/de/python-net/aspose.cells/cell/is_error_value) | Überprüft, ob der Wert dieser Zelle ein Fehler ist.|
| [is_numeric_value](/cells/de/python-net/aspose.cells/cell/is_numeric_value) | Gibt an, ob der innere Wert dieser Zelle numerisch ist (int, double und datetime)|
| [string_value](/cells/de/python-net/aspose.cells/cell/string_value) | Ruft den in der Zelle enthaltenen Zeichenfolgenwert ab. Wenn der Typ dieser Zelle eine Zeichenfolge ist, geben Sie den Zeichenfolgenwert selbst zurück.<br/>Für andere Zelltypen wird der formatierte Zeichenfolgenwert (formatiert mit dem angegebenen Stil dieser Zelle) zurückgegeben.<br/>Der formatierte Zellenwert ist derselbe wie der, den Sie aus Excel erhalten, wenn Sie eine Zelle als Text kopieren (z<br/> Zelle in Texteditor kopieren oder in CSV exportieren).|
| [string_value_without_format](/cells/de/python-net/aspose.cells/cell/string_value_without_format) | Ruft den Wert der Zelle als Zeichenfolge ohne Format ab.|
| [number_category_type](/cells/de/python-net/aspose.cells/cell/number_category_type) |Stellt den Kategorietyp der Zahlenformatierung dieser Zelle dar.|
| [display_string_value](/cells/de/python-net/aspose.cells/cell/display_string_value) | Ruft den formatierten Zeichenfolgenwert dieser Zelle nach Anzeigestil der Zelle ab.|
| [int_value](/cells/de/python-net/aspose.cells/cell/int_value) | Ruft den in der Zelle enthaltenen ganzzahligen Wert ab.|
| [double_value](/cells/de/python-net/aspose.cells/cell/double_value) | Ruft den in der Zelle enthaltenen Double-Wert ab.|
| [float_value](/cells/de/python-net/aspose.cells/cell/float_value) | Ruft den in der Zelle enthaltenen Gleitkommawert ab.|
| [bool_value](/cells/de/python-net/aspose.cells/cell/bool_value) | Ruft den in der Zelle enthaltenen booleschen Wert ab.|
| [has_custom_style](/cells/de/python-net/aspose.cells/cell/has_custom_style) | Gibt an, ob diese Zelle benutzerdefinierte Stileinstellungen hat (anders als die standardmäßig geerbten<br/> aus der entsprechenden Zeile, Spalte oder Arbeitsmappe).|
| [shared_style_index](/cells/de/python-net/aspose.cells/cell/shared_style_index) | Ruft den gemeinsam genutzten Stilindex der Zelle im Stilpool ab.|
| [formula](/cells/de/python-net/aspose.cells/cell/formula) | Ruft eine Formel von [Cell](/cells/de/python-net/aspose.cells/cell) ab oder legt diese fest.|
| [formula_local](/cells/de/python-net/aspose.cells/cell/formula_local) | Rufen Sie die gebietsschemaformatierte Formel der Zelle ab.|
| [r1c1_formula](/cells/de/python-net/aspose.cells/cell/r1c1_formula) | Ruft eine R1C1-Formel von [Cell](/cells/de/python-net/aspose.cells/cell) ab oder legt sie fest.|
| [contains_external_link](/cells/de/python-net/aspose.cells/cell/contains_external_link) | Gibt an, ob diese Zelle einen externen Link enthält.<br/> Gilt nur, wenn die Zelle eine Formelzelle ist.|
| [is_array_header](/cells/de/python-net/aspose.cells/cell/is_array_header) |Gibt an, dass die Formel der Zelle eine Matrixformel ist<br/> und es ist die erste Zelle des Arrays.|
| [is_dynamic_array_formula](/cells/de/python-net/aspose.cells/cell/is_dynamic_array_formula) | Gibt an, ob die Formel der Zelle eine dynamische Array-Formel (true) oder eine Legacy-Array-Formel (false) ist.|
| [is_array_formula](/cells/de/python-net/aspose.cells/cell/is_array_formula) | Gibt an, ob die Zellformel eine Matrixformel ist.|
| [is_in_array](/cells/de/python-net/aspose.cells/cell/is_in_array) | Gibt an, ob die Zellformel eine Matrixformel ist.|
| [is_shared_formula](/cells/de/python-net/aspose.cells/cell/is_shared_formula) |Gibt an, ob die Zellformel Teil einer freigegebenen Formel ist.|
| [is_table_formula](/cells/de/python-net/aspose.cells/cell/is_table_formula) | Gibt an, ob diese Zelle Teil einer Tabellenformel ist.|
| [is_in_table](/cells/de/python-net/aspose.cells/cell/is_in_table) | Gibt an, ob diese Zelle Teil einer Tabellenformel ist.|
| [value](/cells/de/python-net/aspose.cells/cell/value) | Ruft den in dieser Zelle enthaltenen Wert ab.|
| [is_style_set](/cells/de/python-net/aspose.cells/cell/is_style_set) | Gibt an, ob der Stil der Zelle festgelegt ist. Wenn false zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat.|
| [is_merged](/cells/de/python-net/aspose.cells/cell/is_merged) | Überprüft, ob eine Zelle Teil eines zusammengeführten Bereichs ist oder nicht.|
| [comment](/cells/de/python-net/aspose.cells/cell/comment) | Ruft den Kommentar dieser Zelle ab.|
| [html_string](/cells/de/python-net/aspose.cells/cell/html_string) | Ruft die HTML-Zeichenfolge ab und legt sie fest, die Daten und einige Formate in dieser Zelle enthält.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [calculate(options)](/cells/de/python-net/aspose.cells/cell/calculate/#CalculationOptions) | Berechnet die Formel der Zelle.|
| [calculate(ignore_error, custom_function)](/cells/de/python-net/aspose.cells/cell/calculate/#bool-ICustomFunction) | Berechnet die Formel der Zelle.|
| [put_value(bool_value)](/cells/de/python-net/aspose.cells/cell/put_value/#bool) | Fügt einen booleschen Wert in die Zelle ein.|
| [put_value(int_value)](/cells/de/python-net/aspose.cells/cell/put_value/#int) | Fügt einen ganzzahligen Wert in die Zelle ein.|
| [put_value(double_value)](/cells/de/python-net/aspose.cells/cell/put_value/#float) | Fügt einen doppelten Wert in die Zelle ein.|
| [put_value(string_value, is_converted, set_style)](/cells/de/python-net/aspose.cells/cell/put_value/#str-bool-bool) | Fügt einen Wert in die Zelle ein, gegebenenfalls wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle wird zurückgesetzt.|
| [put_value(string_value, is_converted)](/cells/de/python-net/aspose.cells/cell/put_value/#str-bool) | Fügt einen Zeichenfolgenwert in die Zelle ein und konvertiert den Wert gegebenenfalls in einen anderen Datentyp.|
| [put_value(string_value)](/cells/de/python-net/aspose.cells/cell/put_value/#str) | Fügt einen Zeichenfolgenwert in die Zelle ein.|
| [put_value(date_time)](/cells/de/python-net/aspose.cells/cell/put_value/#DateTime) | Fügt einen DateTime-Wert in die Zelle ein.|
| [put_value(object_value)](/cells/de/python-net/aspose.cells/cell/put_value/#any) | Fügt einen Objektwert in die Zelle ein.|
| [get_display_style()](/cells/de/python-net/aspose.cells/cell/get_display_style/#) | Ruft den Anzeigestil der Zelle ab.<br/>Wenn diese Zelle auch von anderen Einstellungen wie bedingter Formatierung, Listenobjekten usw. betroffen ist,<br/> dann kann sich der Anzeigestil von cell.GetStyle() unterscheiden.|
| [get_display_style(include_merged_borders)](/cells/de/python-net/aspose.cells/cell/get_display_style/#bool) | Ruft den Anzeigestil der Zelle ab.<br/> Wenn die Zelle bedingt formatiert ist, ist der Anzeigestil nicht der gleiche wie bei cell.GetStyle().|
| [get_style()](/cells/de/python-net/aspose.cells/cell/get_style/#) | Ruft den Zellenstil ab.|
| [get_style(check_borders)](/cells/de/python-net/aspose.cells/cell/get_style/#bool) | Wenn checkBorders wahr ist, prüfen Sie, ob die Rahmen anderer Zellen den Stil dieser Zelle beeinflussen.|
| [set_style(style)](/cells/de/python-net/aspose.cells/cell/set_style/#Style) | Legt den Zellenstil fest.|
| [set_style(style, explicit_flag)](/cells/de/python-net/aspose.cells/cell/set_style/#Style-bool) | Wenden Sie den Zellenstil an.|
| [set_style(style, flag)](/cells/de/python-net/aspose.cells/cell/set_style/#Style-StyleFlag) | Wenden Sie den Zellenstil an.|
| [set_formula(formula, value)](/cells/de/python-net/aspose.cells/cell/set_formula/#str-any) |Stellen Sie die Formel und den Wert der Formel ein.|
| [set_formula(formula, is_r1c1, is_local, value)](/cells/de/python-net/aspose.cells/cell/set_formula/#str-bool-bool-any) |Stellen Sie die Formel und den Wert der Formel ein.|
| [set_formula(formula, options, value)](/cells/de/python-net/aspose.cells/cell/set_formula/#str-FormulaParseOptions-any) |Stellen Sie die Formel und den Wert der Formel ein.|
| [set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local)](/cells/de/python-net/aspose.cells/cell/set_array_formula/#str-int-int-bool-bool) | Legt eine Matrixformel auf einen Zellbereich fest.|
| [set_array_formula(array_formula, row_number, column_number)](/cells/de/python-net/aspose.cells/cell/set_array_formula/#str-int-int) | Legt eine Array-Formel (alte Array-Formel, die über STRG+UMSCHALT+EINGABETASTE in MS Excel eingegeben wurde) auf einen Bereich von Zellen fest.|
| [set_array_formula(array_formula, row_number, column_number, options)](/cells/de/python-net/aspose.cells/cell/set_array_formula/#str-int-int-FormulaParseOptions) | Legt eine Matrixformel auf einen Zellbereich fest.|
| [set_array_formula(array_formula, row_number, column_number, options, values)](/cells/de/python-net/aspose.cells/cell/set_array_formula/#str-int-int-FormulaParseOptions-list) | Legt eine Matrixformel auf einen Zellbereich fest.|
| [set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local)](/cells/de/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-bool-bool) | Legt eine Formel auf einen Zellbereich fest.|
| [set_shared_formula(shared_formula, row_number, column_number)](/cells/de/python-net/aspose.cells/cell/set_shared_formula/#str-int-int) | Legt freigegebene Formeln auf einen Zellbereich fest.|
| [set_shared_formula(shared_formula, row_number, column_number, options)](/cells/de/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-FormulaParseOptions) | Legt freigegebene Formeln auf einen Zellbereich fest.|
| [set_shared_formula(shared_formula, row_number, column_number, options, values)](/cells/de/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-FormulaParseOptions-list) | Legt freigegebene Formeln auf einen Zellbereich fest.|
| [get_leafs()](/cells/de/python-net/aspose.cells/cell/get_leafs/#) | Rufen Sie alle Zellen ab, die direkt auf diese Zelle verweisen und aktualisiert werden müssen, wenn diese Zelle geändert wird.|
| [get_leafs(recursive)](/cells/de/python-net/aspose.cells/cell/get_leafs/#bool) | Holen Sie sich alle Zellen, die aktualisiert werden, wenn diese Zelle geändert wird.|
| [set_dynamic_array_formula(array_formula, options, calculate_value)](/cells/de/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-bool) | Legt eine dynamische Matrixformel fest und lässt die Formel nach Möglichkeit in benachbarte Zellen übergehen.|
| [set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value)](/cells/de/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-list-bool-bool) | Legt eine dynamische Matrixformel fest und lässt die Formel nach Möglichkeit in benachbarte Zellen übergehen.|
| [set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts)](/cells/de/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-list-bool-bool-CalculationOptions) | Legt eine dynamische Matrixformel fest und lässt die Formel nach Möglichkeit in benachbarte Zellen übergehen.|
| [set_table_formula(row_number, column_number, row_input_cell, column_input_cell, values)](/cells/de/python-net/aspose.cells/cell/set_table_formula/#int-int-str-str-list) | Erstellen Sie eine Datentabelle mit zwei Variablen für einen bestimmten Bereich, beginnend mit dieser Zelle.|
| [set_table_formula(row_number, column_number, input_cell, is_row_input, values)](/cells/de/python-net/aspose.cells/cell/set_table_formula/#int-int-str-bool-list) | Erstellen Sie eine Datentabelle mit einer Variablen für einen bestimmten Bereich, beginnend mit dieser Zelle.|
| [set_table_formula(row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values)](/cells/de/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-int-int-list) | Erstellen Sie eine Datentabelle mit zwei Variablen für einen bestimmten Bereich, beginnend mit dieser Zelle.|
| [set_table_formula(row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values)](/cells/de/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-bool-list) | Erstellen Sie eine Datentabelle mit einer Variablen für einen bestimmten Bereich, beginnend mit dieser Zelle.|
| [get_characters()](/cells/de/python-net/aspose.cells/cell/get_characters/#) | Gibt alle Characters-Objekte zurück<br/> das einen Bereich von Zeichen innerhalb des Zellentextes darstellt.|
| [get_characters(flag)](/cells/de/python-net/aspose.cells/cell/get_characters/#bool) | Gibt alle Characters-Objekte zurück<br/> das einen Bereich von Zeichen innerhalb des Zellentextes darstellt.|
| [get_string_value(format_strategy)](/cells/de/python-net/aspose.cells/cell/get_string_value/#CellValueFormatStrategy) | Ruft den Zeichenfolgenwert durch eine bestimmte formatierte Strategie ab.|
| [get_width_of_value()](/cells/de/python-net/aspose.cells/cell/get_width_of_value/#) |Ruft die Breite des Werts in Pixeln ab.|
| [get_height_of_value()](/cells/de/python-net/aspose.cells/cell/get_height_of_value/#) | Ruft die Höhe des Werts in Pixeln ab.|
| [get_format_conditions()](/cells/de/python-net/aspose.cells/cell/get_format_conditions/#) | Ruft Formatbedingungen ab, die für diese Zelle gelten.|
| [get_formula(is_r1c1, is_local)](/cells/de/python-net/aspose.cells/cell/get_formula/#bool-bool) | Holen Sie sich die Formel dieser Zelle.|
| [get_precedents()](/cells/de/python-net/aspose.cells/cell/get_precedents/#) | Ruft alle Verweise ab, die in der Formel dieser Zelle vorkommen.|
| [get_dependents(is_all)](/cells/de/python-net/aspose.cells/cell/get_dependents/#bool) | Holen Sie sich alle Zellen, deren Formel direkt auf diese Zelle verweist.|
| [get_precedents_in_calculation()](/cells/de/python-net/aspose.cells/cell/get_precedents_in_calculation/#) | Ruft alle Präzedenzfälle (Verweis auf Zellen in der aktuellen Arbeitsmappe) ab, die von der Formel dieser Zelle während der Berechnung verwendet werden.|
| [get_dependents_in_calculation(recursive)](/cells/de/python-net/aspose.cells/cell/get_dependents_in_calculation/#bool) |Ruft alle Zellen ab, deren berechnetes Ergebnis von dieser Zelle abhängt.|
| [get_array_range()](/cells/de/python-net/aspose.cells/cell/get_array_range/#) | Ruft den Matrixbereich ab, wenn die Formel der Zelle eine Matrixformel ist.|
| [remove_array_formula(leave_normal_formula)](/cells/de/python-net/aspose.cells/cell/remove_array_formula/#bool) | Matrixformel entfernen.|
| [copy(cell)](/cells/de/python-net/aspose.cells/cell/copy/#Cell) | Kopiert Daten aus einer Quellzelle.|
| [characters(start_index, length)](/cells/de/python-net/aspose.cells/cell/characters/#int-int) | Gibt ein Characters-Objekt zurück, das einen Bereich von Zeichen im Zelltext darstellt.|
| [is_rich_text()](/cells/de/python-net/aspose.cells/cell/is_rich_text/#) | Gibt an, ob der Zellzeichenfolgewert ein Rich-Text ist.|
| [set_characters(characters)](/cells/de/python-net/aspose.cells/cell/set_characters/#list) | Legt das Rich-Text-Format der Zelle fest.|
| [get_merged_range()](/cells/de/python-net/aspose.cells/cell/get_merged_range/#) | Gibt ein [Range](/cells/de/python-net/aspose.cells/range)-Objekt zurück, das einen zusammengeführten Bereich darstellt.|
| [get_html_string(html5)](/cells/de/python-net/aspose.cells/cell/get_html_string/#bool) | Ruft die HTML-Zeichenfolge ab, die Daten und einige Formate in dieser Zelle enthält.|
| [to_json()](/cells/de/python-net/aspose.cells/cell/to_json/#) | Konvertieren Sie [Cell](/cells/de/python-net/aspose.cells/cell) in JSON-Strukturdaten.|
| [equals(cell)](/cells/de/python-net/aspose.cells/cell/equals/#Cell) | Überprüft, ob dieses Objekt mit einem anderen Zellobjekt auf dieselbe Zelle verweist.|
| [get_conditional_formatting_result()](/cells/de/python-net/aspose.cells/cell/get_conditional_formatting_result/#) | Holen Sie sich das Ergebnis der bedingten Formatierung.|
| [get_validation()](/cells/de/python-net/aspose.cells/cell/get_validation/#) | Ruft die auf diese Zelle angewendete Validierung ab.|
| [get_validation_value()](/cells/de/python-net/aspose.cells/cell/get_validation_value/#) | Ruft den Validierungswert ab, der auf diese Zelle angewendet wurde.|
| [get_table()](/cells/de/python-net/aspose.cells/cell/get_table/#) | Ruft die Tabelle ab, die diese Zelle enthält.|



###  Beispiel

```python
from aspose.cells import TextAlignmentType, Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
# Put a string into a cell
cell = cells.get(0, 0)
cell.put_value("Hello")
first = cell.string_value
# Put an integer into a cell
cell = cells.get("B1")
cell.put_value(12)
second = cell.int_value
# Put a double into a cell
cell = cells.get(0, 2)
cell.put_value(-1.234)
third = cell.double_value
# Put a formula into a cell
cell = cells.get("D1")
cell.formula = "=B1 + C1"
# Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells.get("b2")
cell.formula = "=sum(average(b1,c1), b1)"
# Set style of a cell
style = cell.get_style()
# Set background color
style.background_color = Color.yellow
# Set format of a cell
style.font.name = "Courier New"
style.vertical_alignment = TextAlignmentType.TOP
cell.set_style(style)

```

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
* Klasse [Range](/cells/de/python-net/aspose.cells/range)
