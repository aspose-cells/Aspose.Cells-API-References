---
title: ValidationCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1550
url: /fr/python-net/aspose.cells/validationcollection/
is_root: false
---
##  ValidationCollection classe
Représente la collecte de validation des données.



Le type ValidationCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells/validationcollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add()](/cells/fr/python-net/aspose.cells/validationcollection/add/#) |Ajoute une validation de données à la collection.|
| [add(ca)](/cells/fr/python-net/aspose.cells/validationcollection/add/#CellArea) |Ajoute une validation de données à la collection.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells/validationcollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells/validationcollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells/validationcollection/index_of/#Validation-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells/validationcollection/index_of/#Validation-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells/validationcollection/last_index_of/#Validation) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [remove_a_cell(row, column)](/cells/fr/python-net/aspose.cells/validationcollection/remove_a_cell/#int-int) | Supprime tous les paramètres de validation de la cellule.|
| [remove_area(ca)](/cells/fr/python-net/aspose.cells/validationcollection/remove_area/#CellArea) | Supprime tous les paramètres de validation sur la plage.|
| [get_validation_in_cell(row, column)](/cells/fr/python-net/aspose.cells/validationcollection/get_validation_in_cell/#int-int) | Obtient la validation appliquée à la cellule donnée.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells/validationcollection/binary_search/#Validation) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import CellArea, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.LIST
validation.formula1 = "a,b,c,d"

```

###  Voir également
* module [aspose.cells](..)
