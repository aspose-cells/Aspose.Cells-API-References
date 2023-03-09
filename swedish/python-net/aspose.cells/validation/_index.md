---
title: Validation klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1540
url: /sv/python-net/aspose.cells/validation/
is_root: false
---
##  Validation klass
Representerar datavalidering.inställningar.



Typen Validation avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [operator](/cells/sv/python-net/aspose.cells/validation/operator) | Representerar operatören för datavalideringen.|
| [alert_style](/cells/sv/python-net/aspose.cells/validation/alert_style) | Representerar valideringsvarningsstilen.|
| [type](/cells/sv/python-net/aspose.cells/validation/type) | Representerar datavalideringstypen.|
| [input_message](/cells/sv/python-net/aspose.cells/validation/input_message) | Representerar inmatningsmeddelandet för datavalidering.|
| [input_title](/cells/sv/python-net/aspose.cells/validation/input_title) | Representerar titeln på dialogrutan för datavalidering.|
| [error_message](/cells/sv/python-net/aspose.cells/validation/error_message) | Representerar datavalideringsfelmeddelandet.|
| [error_title](/cells/sv/python-net/aspose.cells/validation/error_title) | Representerar titeln på dialogrutan för datavalideringsfel.|
| [show_input](/cells/sv/python-net/aspose.cells/validation/show_input) |Indikerar om inmatningsmeddelandet för datavalidering kommer att visas när användaren väljer en cell i datavalideringsintervallet.|
| [show_error](/cells/sv/python-net/aspose.cells/validation/show_error) | Indikerar om datavalideringsfelmeddelandet kommer att visas när användaren anger ogiltiga data.|
| [ignore_blank](/cells/sv/python-net/aspose.cells/validation/ignore_blank) | Indikerar om tomma värden är tillåtna av intervalldatavalideringen.|
| [formula1](/cells/sv/python-net/aspose.cells/validation/formula1) | Representerar värdet eller uttrycket som är associerat med datavalideringen.|
| [formula2](/cells/sv/python-net/aspose.cells/validation/formula2) | Representerar värdet eller uttrycket som är associerat med datavalideringen.|
| [value1](/cells/sv/python-net/aspose.cells/validation/value1) | Representerar det första värdet som är kopplat till datavalideringen.|
| [value2](/cells/sv/python-net/aspose.cells/validation/value2) | Representerar det andra värdet som är associerat med datavalideringen.|
| [in_cell_drop_down](/cells/sv/python-net/aspose.cells/validation/in_cell_drop_down) | Anger om datavalidering visar en rullgardinslista som innehåller acceptabla värden.|
| [areas](/cells/sv/python-net/aspose.cells/validation/areas) | Hämtar alla [CellArea](/cells/sv/python-net/aspose.cells/cellarea) som innehåller datavalideringsinställningarna.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/sv/python-net/aspose.cells/validation/get_formula1/#bool-bool) | Hämtar värdet eller uttrycket som är kopplat till denna validering.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/sv/python-net/aspose.cells/validation/get_formula1/#bool-bool-int-int) | Hämtar värdet eller uttrycket som är associerat med denna validering för den specifika cellen.|
| [get_formula2(is_r1c1, is_local)](/cells/sv/python-net/aspose.cells/validation/get_formula2/#bool-bool) | Hämtar värdet eller uttrycket som är kopplat till denna validering.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/sv/python-net/aspose.cells/validation/get_formula2/#bool-bool-int-int) | Hämtar värdet eller uttrycket som är associerat med denna validering för den specifika cellen.|
| [add_area(cell_area)](/cells/sv/python-net/aspose.cells/validation/add_area/#CellArea) | Tillämpar valideringen på området.|
| [add_area(cell_area, check_intersection, check_edge)](/cells/sv/python-net/aspose.cells/validation/add_area/#CellArea-bool-bool) | Tillämpar valideringen på området.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/sv/python-net/aspose.cells/validation/set_formula1/#str-bool-bool) | Ställer in värdet eller uttrycket som är associerat med denna validering.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/sv/python-net/aspose.cells/validation/set_formula2/#str-bool-bool) | Ställer in värdet eller uttrycket som är associerat med denna validering.|
| [get_list_value(row, column)](/cells/sv/python-net/aspose.cells/validation/get_list_value/#int-int) |Hämta värdet för lista för valideringen för den angivna cellen.|
| [add_areas(areas, check_intersection, check_edge)](/cells/sv/python-net/aspose.cells/validation/add_areas/#list-bool-bool) | Tillämpar valideringen på givna områden.|
| [remove_area(cell_area)](/cells/sv/python-net/aspose.cells/validation/remove_area/#CellArea) | Ta bort valideringsinställningarna i intervallet.|
| [remove_areas(areas)](/cells/sv/python-net/aspose.cells/validation/remove_areas/#list) | Tar bort denna validering från givna områden.|
| [remove_a_cell(row, column)](/cells/sv/python-net/aspose.cells/validation/remove_a_cell/#int-int) | Ta bort valideringsinställningarna i cellen.|
| [copy(source, copy_option)](/cells/sv/python-net/aspose.cells/validation/copy/#Validation-CopyOptions) | Kopia validering.|



###  Exempel

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

###  Se även
* modul [aspose.cells](..)
* klass [CellArea](/cells/sv/python-net/aspose.cells/cellarea)
