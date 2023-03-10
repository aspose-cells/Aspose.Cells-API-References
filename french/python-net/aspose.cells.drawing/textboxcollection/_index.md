---
title: TextBoxCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 690
url: /fr/python-net/aspose.cells.drawing/textboxcollection/
is_root: false
---
##  TextBoxCollection classe
Encapsule une collection de [TextBox](/cells/fr/python-net/aspose.cells.drawing/textbox) objets.



Le type TextBoxCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [copy_to(array)](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/index_of/#TextBox-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/index_of/#TextBox-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [add(upper_left_row, upper_left_column, height, width)](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/add/#int-int-int-int) |Ajoute une zone de texte à la collection.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.drawing/textboxcollection/binary_search/#TextBox) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get collection object
textBoxCollection = workbook.worksheets[0].text_boxes
# add a textbox
textBoxCollection.add(1, 1, 50, 100)
for tbox in textBoxCollection:
    pass

```

###  Voir également
* module [aspose.cells.drawing](..)
* classe [TextBox](/cells/fr/python-net/aspose.cells.drawing/textbox)
