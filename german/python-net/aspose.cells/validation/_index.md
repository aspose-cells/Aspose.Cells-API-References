---
title: Validation Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1540
url: /de/python-net/aspose.cells/validation/
is_root: false
---
##  Validation Klasse
Repräsentiert Datenvalidierung.Einstellungen.



Der Typ Validation macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [operator](/cells/de/python-net/aspose.cells/validation/operator) | Stellt den Operator für die Datenvalidierung dar.|
| [alert_style](/cells/de/python-net/aspose.cells/validation/alert_style) | Stellt den Validierungswarnungsstil dar.|
| [type](/cells/de/python-net/aspose.cells/validation/type) | Stellt den Datenvalidierungstyp dar.|
| [input_message](/cells/de/python-net/aspose.cells/validation/input_message) | Stellt die Datenvalidierungs-Eingabenachricht dar.|
| [input_title](/cells/de/python-net/aspose.cells/validation/input_title) | Stellt den Titel des Eingabedialogfelds zur Datenvalidierung dar.|
| [error_message](/cells/de/python-net/aspose.cells/validation/error_message) | Stellt die Fehlermeldung zur Datenvalidierung dar.|
| [error_title](/cells/de/python-net/aspose.cells/validation/error_title) | Stellt den Titel des Datenüberprüfungsfehlerdialogfelds dar.|
| [show_input](/cells/de/python-net/aspose.cells/validation/show_input) |Gibt an, ob die Datenüberprüfungs-Eingabemeldung angezeigt wird, wenn der Benutzer eine Zelle im Datenüberprüfungsbereich auswählt.|
| [show_error](/cells/de/python-net/aspose.cells/validation/show_error) | Gibt an, ob die Datenüberprüfungsfehlermeldung angezeigt wird, wenn der Benutzer ungültige Daten eingibt.|
| [ignore_blank](/cells/de/python-net/aspose.cells/validation/ignore_blank) | Gibt an, ob bei der Bereichsdatenvalidierung Leerwerte zulässig sind.|
| [formula1](/cells/de/python-net/aspose.cells/validation/formula1) | Stellt den Wert oder Ausdruck dar, der der Datenvalidierung zugeordnet ist.|
| [formula2](/cells/de/python-net/aspose.cells/validation/formula2) | Stellt den Wert oder Ausdruck dar, der der Datenvalidierung zugeordnet ist.|
| [value1](/cells/de/python-net/aspose.cells/validation/value1) | Stellt den ersten Wert dar, der der Datenvalidierung zugeordnet ist.|
| [value2](/cells/de/python-net/aspose.cells/validation/value2) | Stellt den zweiten Wert dar, der der Datenvalidierung zugeordnet ist.|
| [in_cell_drop_down](/cells/de/python-net/aspose.cells/validation/in_cell_drop_down) | Gibt an, ob die Datenvalidierung eine Dropdown-Liste anzeigt, die akzeptable Werte enthält.|
| [areas](/cells/de/python-net/aspose.cells/validation/areas) | Ruft alle [CellArea](/cells/de/python-net/aspose.cells/cellarea) ab, die die Datenüberprüfungseinstellungen enthalten.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/de/python-net/aspose.cells/validation/get_formula1/#bool-bool) | Ruft den Wert oder Ausdruck ab, der dieser Validierung zugeordnet ist.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/de/python-net/aspose.cells/validation/get_formula1/#bool-bool-int-int) | Ruft den Wert oder Ausdruck ab, der dieser Validierung für eine bestimmte Zelle zugeordnet ist.|
| [get_formula2(is_r1c1, is_local)](/cells/de/python-net/aspose.cells/validation/get_formula2/#bool-bool) | Ruft den Wert oder Ausdruck ab, der dieser Validierung zugeordnet ist.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/de/python-net/aspose.cells/validation/get_formula2/#bool-bool-int-int) | Ruft den Wert oder Ausdruck ab, der dieser Validierung für eine bestimmte Zelle zugeordnet ist.|
| [add_area(cell_area)](/cells/de/python-net/aspose.cells/validation/add_area/#CellArea) | Wendet die Validierung auf den Bereich an.|
| [add_area(cell_area, check_intersection, check_edge)](/cells/de/python-net/aspose.cells/validation/add_area/#CellArea-bool-bool) | Wendet die Validierung auf den Bereich an.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/de/python-net/aspose.cells/validation/set_formula1/#str-bool-bool) | Legt den Wert oder Ausdruck fest, der dieser Validierung zugeordnet ist.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/de/python-net/aspose.cells/validation/set_formula2/#str-bool-bool) | Legt den Wert oder Ausdruck fest, der dieser Validierung zugeordnet ist.|
| [get_list_value(row, column)](/cells/de/python-net/aspose.cells/validation/get_list_value/#int-int) |Rufen Sie den Wert für die Liste der Validierung für die angegebene Zelle ab.|
| [add_areas(areas, check_intersection, check_edge)](/cells/de/python-net/aspose.cells/validation/add_areas/#list-bool-bool) | Wendet die Validierung auf bestimmte Bereiche an.|
| [remove_area(cell_area)](/cells/de/python-net/aspose.cells/validation/remove_area/#CellArea) | Entfernen Sie die Validierungseinstellungen im Bereich.|
| [remove_areas(areas)](/cells/de/python-net/aspose.cells/validation/remove_areas/#list) | Entfernt diese Validierung aus bestimmten Bereichen.|
| [remove_a_cell(row, column)](/cells/de/python-net/aspose.cells/validation/remove_a_cell/#int-int) | Entfernen Sie die Validierungseinstellungen in der Zelle.|
| [copy(source, copy_option)](/cells/de/python-net/aspose.cells/validation/copy/#Validation-CopyOptions) | Validierung kopieren.|



###  Beispiel

```python
from aspose.cells import CellArea, OperatorType, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.WHOLE_NUMBER
validation.operator = OperatorType.BETWEEN
validation.formula1 = "3"
validation.formula2 = "1234"

```

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [CellArea](/cells/de/python-net/aspose.cells/cellarea)
