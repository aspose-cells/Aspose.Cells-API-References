---
title: ConditionalFormattingIconCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 320
url: /fr/python-net/aspose.cells/conditionalformattingiconcollection/
is_root: false
---
##  ConditionalFormattingIconCollection classe
Représente une collection de [ConditionalFormattingIcon](/cells/fr/python-net/aspose.cells/conditionalformattingicon) objets.



Le type ConditionalFormattingIconCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(type, index)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/add/#IconSetType-int) | Ajoute l'objet [ConditionalFormattingIcon](/cells/fr/python-net/aspose.cells/conditionalformattingicon).|
| [add(cficon)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/add/#ConditionalFormattingIcon) | Ajoute l'objet [ConditionalFormattingIcon](/cells/fr/python-net/aspose.cells/conditionalformattingicon).|
| [copy_to(array)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/copy_to/#int-list-int-int) | Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/index_of/#ConditionalFormattingIcon-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/index_of/#ConditionalFormattingIcon-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/last_index_of/#ConditionalFormattingIcon) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/last_index_of/#ConditionalFormattingIcon-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/last_index_of/#ConditionalFormattingIcon-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells/conditionalformattingiconcollection/binary_search/#ConditionalFormattingIcon) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import CellArea, FormatConditionType, IconSetType, Workbook

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Get Conditional Formatting
cformattings = sheet.conditional_formattings
# Adds an empty conditional formatting
index = cformattings.add()
# Get newly added Conditional formatting
fcs = cformattings[index]
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
# Sets condition
idx = fcs.add_condition(FormatConditionType.ICON_SET)
cond = fcs[idx]
# Sets condition's type
cond.icon_set.type = IconSetType.ARROWS_GRAY3
# Add custom iconset condition.
cfIcon = cond.icon_set.cf_icons[0]
cfIcon.type = IconSetType.ARROWS3
cfIcon.index = 0
cfIcon1 = cond.icon_set.cf_icons[1]
cfIcon1.type = IconSetType.ARROWS_GRAY3
cfIcon1.index = 1
cfIcon2 = cond.icon_set.cf_icons[2]
cfIcon2.type = IconSetType.BOXES5
cfIcon2.index = 2
# Saving the Excel file
workbook.save("output.xls")

```

###  Voir également
* module [aspose.cells](..)
* classe [ConditionalFormattingIcon](/cells/fr/python-net/aspose.cells/conditionalformattingicon)
