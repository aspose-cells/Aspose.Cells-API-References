---
title: FormatConditionCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 700
url: /fr/python-net/aspose.cells/formatconditioncollection/
is_root: false
---
##  FormatConditionCollection classe
Représente la mise en forme conditionnelle.
Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels.



Le type FormatConditionCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [count](/cells/fr/python-net/aspose.cells/formatconditioncollection/count) | Obtient le nombre de conditions.|
| [range_count](/cells/fr/python-net/aspose.cells/formatconditioncollection/range_count) | Obtient le nombre de plages mises en forme de manière conditionnelle.|



Obtient la condition de mise en forme par index.
###  Indexeur
| Nom| Description|
| :- | :- |
| [index] | l'index de la condition de formatage à renvoyer.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add_condition(type, operator_type, formula1, formula2)](/cells/fr/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType-OperatorType-str-str) | Ajoute une condition de formatage.|
| [add_condition(type)](/cells/fr/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType) |Ajoutez une condition de mise en forme.|
| [remove_area(index)](/cells/fr/python-net/aspose.cells/formatconditioncollection/remove_area/#int) | Supprime la plage de cellules mise en forme conditionnelle par index.|
| [remove_area(start_row, start_column, total_rows, total_columns)](/cells/fr/python-net/aspose.cells/formatconditioncollection/remove_area/#int-int-int-int) | Supprimez la mise en forme conditionnelle dans la plage.|
| [add(cell_area, type, operator_type, formula1, formula2)](/cells/fr/python-net/aspose.cells/formatconditioncollection/add/#CellArea-FormatConditionType-OperatorType-str-str) | Ajoute une condition de formatage et une plage de cellules affectée aux FormatConditions<br/>Les FormatConditions peuvent contenir jusqu'à trois formats conditionnels.<br/> Les références aux autres feuilles ne sont pas autorisées dans les formules de mise en forme conditionnelle.|
| [add_area(cell_area)](/cells/fr/python-net/aspose.cells/formatconditioncollection/add_area/#CellArea) | Ajoute une plage de cellules mise en forme de manière conditionnelle.|
| [get_cell_area(index)](/cells/fr/python-net/aspose.cells/formatconditioncollection/get_cell_area/#int) | Obtient la plage de cellules mise en forme de manière conditionnelle par index.|
| [remove_condition(index)](/cells/fr/python-net/aspose.cells/formatconditioncollection/remove_condition/#int) | Supprime la condition de formatage par index.|



###  Exemples

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Create a new Workbook.
workbook = Workbook()
# Get the first worksheet.
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

###  Voir également
* module [aspose.cells](..)
