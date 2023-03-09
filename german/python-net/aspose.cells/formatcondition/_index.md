---
title: FormatCondition Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 690
url: /de/python-net/aspose.cells/formatcondition/
is_root: false
---
##  FormatCondition Klasse
Stellt die Bedingung für die bedingte Formatierung dar.



Der Typ FormatCondition macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [formula1](/cells/de/python-net/aspose.cells/formatcondition/formula1) | Ruft den Wert oder Ausdruck ab, der der bedingten Formatierung zugeordnet ist, und legt diesen fest.|
| [formula2](/cells/de/python-net/aspose.cells/formatcondition/formula2) | Ruft den Wert oder Ausdruck ab, der der bedingten Formatierung zugeordnet ist, und legt diesen fest.|
| [operator](/cells/de/python-net/aspose.cells/formatcondition/operator) | Ruft den Typ des bedingten Formatoperators ab und legt ihn fest.|
| [stop_if_true](/cells/de/python-net/aspose.cells/formatcondition/stop_if_true) |True, keine Regeln mit niedrigerer Priorität können auf diese Regel angewendet werden, wenn diese Regel als wahr ausgewertet wird.<br/> Gilt nur für Excel 2007;|
| [priority](/cells/de/python-net/aspose.cells/formatcondition/priority) | Die Priorität dieser Regel zur bedingten Formatierung.<br/>format ausgewertet und gerendert werden sollen. Niedrigere Zahlenwerte haben höhere Priorität als<br/> höhere numerische Werte, wobei '1' die höchste Priorität hat.|
| [style](/cells/de/python-net/aspose.cells/formatcondition/style) | Ruft den Stil von bedingt formatierten Zellbereichen ab oder legt diesen fest.|
| [type](/cells/de/python-net/aspose.cells/formatcondition/type) | Ruft ab und legt fest, ob das bedingte Format Type.|
| [icon_set](/cells/de/python-net/aspose.cells/formatcondition/icon_set) | Rufen Sie die „IconSet“-Instanz der bedingten Formatierung ab.<br/>Der IconSetType der Standardinstanz ist TrafficLights31.<br/> Gültig nur für type = IconSet.|
| [data_bar](/cells/de/python-net/aspose.cells/formatcondition/data_bar) | Rufen Sie die „DataBar“-Instanz der bedingten Formatierung ab.<br/>Die Farbe der Standardinstanz ist blau.<br/> Gültig nur für Typ ist DataBar.|
| [color_scale](/cells/de/python-net/aspose.cells/formatcondition/color_scale) | Rufen Sie die „ColorScale“-Instanz der bedingten Formatierung ab.<br/>Die Standardinstanz ist eine "grün-gelb-rote" 3ColorScale .<br/> Nur gültig für Typ = ColorScale.|
| [top10](/cells/de/python-net/aspose.cells/formatcondition/top10) | Holen Sie sich die „Top10“-Instanz der bedingten Formatierung.<br/>Die Regel der Standardinstanz hebt Zellen hervor, deren<br/>Werte fallen in die Top-10-Klammer.<br/> Gültig nur für Typ ist Top10.|
| [above_average](/cells/de/python-net/aspose.cells/formatcondition/above_average) |Rufen Sie die Instanz „AboveAverage“ der bedingten Formatierung ab.<br/> Die Regel der Standardinstanz hebt Zellen hervor, die sind<br/>über dem Durchschnitt für alle Werte im Bereich.<br/> Nur gültig für Typ = AboveAverage.|
| [text](/cells/de/python-net/aspose.cells/formatcondition/text) | Der Textwert in einer Regel zur bedingten Formatierung „Text enthält“.<br/>Gültig nur für type = containsText, notContainsText, beginWith und endedWith.<br/> Der Standardwert ist null.|
| [time_period](/cells/de/python-net/aspose.cells/formatcondition/time_period) | Der anwendbare Zeitraum in einer bedingten Formatierungsregel „Datum auftritt…“.<br/>Nur gültig für type = timePeriod.<br/> Der Standardwert ist TimePeriodType.Today.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/de/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool) | Ruft den Wert oder Ausdruck ab, der dieser Formatbedingung zugeordnet ist.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/de/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool-int-int) | Ruft den Wert oder Ausdruck der bedingten Formatierung der Zelle ab.|
| [get_formula1(row, column)](/cells/de/python-net/aspose.cells/formatcondition/get_formula1/#int-int) | Ruft die Formel der bedingten Formatierung der Zelle ab.|
| [get_formula2(is_r1c1, is_local)](/cells/de/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool) | Ruft den Wert oder Ausdruck ab, der dieser Formatbedingung zugeordnet ist.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/de/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool-int-int) | Ruft den Wert oder Ausdruck der bedingten Formatierung der Zelle ab.|
| [get_formula2(row, column)](/cells/de/python-net/aspose.cells/formatcondition/get_formula2/#int-int) | Ruft die Formel der bedingten Formatierung der Zelle ab.|
| [set_formulas(formula1, formula2, is_r1c1, is_local)](/cells/de/python-net/aspose.cells/formatcondition/set_formulas/#str-str-bool-bool) | Legt den Wert oder Ausdruck fest, der dieser Formatbedingung zugeordnet ist.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/de/python-net/aspose.cells/formatcondition/set_formula1/#str-bool-bool) | Legt den Wert oder Ausdruck fest, der dieser Formatbedingung zugeordnet ist.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/de/python-net/aspose.cells/formatcondition/set_formula2/#str-bool-bool) | Legt den Wert oder Ausdruck fest, der dieser Formatbedingung zugeordnet ist.|



###  Beispiele

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Adds condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")

```

###  Siehe auch
* Modul [aspose.cells](..)
