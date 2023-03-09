---
title: Validation classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1540
url: /fr/python-net/aspose.cells/validation/
is_root: false
---
##  Validation classe
Représente validation.settings des données.



Le type Validation expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [operator](/cells/fr/python-net/aspose.cells/validation/operator) | Représente l'opérateur pour la validation des données.|
| [alert_style](/cells/fr/python-net/aspose.cells/validation/alert_style) | Représente le style d'alerte de validation.|
| [type](/cells/fr/python-net/aspose.cells/validation/type) | Représente le type de validation des données.|
| [input_message](/cells/fr/python-net/aspose.cells/validation/input_message) | Représente le message d'entrée de validation des données.|
| [input_title](/cells/fr/python-net/aspose.cells/validation/input_title) | Représente le titre de la boîte de dialogue d'entrée de validation des données.|
| [error_message](/cells/fr/python-net/aspose.cells/validation/error_message) | Représente le message d'erreur de validation des données.|
| [error_title](/cells/fr/python-net/aspose.cells/validation/error_title) | Représente le titre de la boîte de dialogue d'erreur de validation des données.|
| [show_input](/cells/fr/python-net/aspose.cells/validation/show_input) |Indique si le message d'entrée de validation des données s'affiche chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données.|
| [show_error](/cells/fr/python-net/aspose.cells/validation/show_error) | Indique si le message d'erreur de validation des données s'affichera chaque fois que l'utilisateur saisira des données non valides.|
| [ignore_blank](/cells/fr/python-net/aspose.cells/validation/ignore_blank) | Indique si les valeurs vides sont autorisées par la validation des données de plage.|
| [formula1](/cells/fr/python-net/aspose.cells/validation/formula1) | Représente la valeur ou l'expression associée à la validation des données.|
| [formula2](/cells/fr/python-net/aspose.cells/validation/formula2) | Représente la valeur ou l'expression associée à la validation des données.|
| [value1](/cells/fr/python-net/aspose.cells/validation/value1) | Représente la première valeur associée à la validation des données.|
| [value2](/cells/fr/python-net/aspose.cells/validation/value2) | Représente la deuxième valeur associée à la validation des données.|
| [in_cell_drop_down](/cells/fr/python-net/aspose.cells/validation/in_cell_drop_down) | Indique si la validation des données affiche une liste déroulante contenant des valeurs acceptables.|
| [areas](/cells/fr/python-net/aspose.cells/validation/areas) | Obtient tous les [CellArea](/cells/fr/python-net/aspose.cells/cellarea) qui contiennent les paramètres de validation des données.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/fr/python-net/aspose.cells/validation/get_formula1/#bool-bool) | Obtient la valeur ou l'expression associée à cette validation.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/fr/python-net/aspose.cells/validation/get_formula1/#bool-bool-int-int) | Obtient la valeur ou l'expression associée à cette validation pour la cellule spécifique.|
| [get_formula2(is_r1c1, is_local)](/cells/fr/python-net/aspose.cells/validation/get_formula2/#bool-bool) | Obtient la valeur ou l'expression associée à cette validation.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/fr/python-net/aspose.cells/validation/get_formula2/#bool-bool-int-int) | Obtient la valeur ou l'expression associée à cette validation pour la cellule spécifique.|
| [add_area(cell_area)](/cells/fr/python-net/aspose.cells/validation/add_area/#CellArea) | Applique la validation à la zone.|
| [add_area(cell_area, check_intersection, check_edge)](/cells/fr/python-net/aspose.cells/validation/add_area/#CellArea-bool-bool) | Applique la validation à la zone.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/fr/python-net/aspose.cells/validation/set_formula1/#str-bool-bool) | Définit la valeur ou l'expression associée à cette validation.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/fr/python-net/aspose.cells/validation/set_formula2/#str-bool-bool) | Définit la valeur ou l'expression associée à cette validation.|
| [get_list_value(row, column)](/cells/fr/python-net/aspose.cells/validation/get_list_value/#int-int) |Obtenez la valeur de la liste de la validation pour la cellule spécifiée.|
| [add_areas(areas, check_intersection, check_edge)](/cells/fr/python-net/aspose.cells/validation/add_areas/#list-bool-bool) | Applique la validation à des zones données.|
| [remove_area(cell_area)](/cells/fr/python-net/aspose.cells/validation/remove_area/#CellArea) | Supprimez les paramètres de validation de la plage.|
| [remove_areas(areas)](/cells/fr/python-net/aspose.cells/validation/remove_areas/#list) | Supprime cette validation des zones données.|
| [remove_a_cell(row, column)](/cells/fr/python-net/aspose.cells/validation/remove_a_cell/#int-int) | Supprimez les paramètres de validation dans la cellule.|
| [copy(source, copy_option)](/cells/fr/python-net/aspose.cells/validation/copy/#Validation-CopyOptions) | Validation de copie.|



###  Exemples

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

###  Voir également
* module [aspose.cells](..)
* classe [CellArea](/cells/fr/python-net/aspose.cells/cellarea)
