---
title: HorizontalPageBreakCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 760
url: /fr/python-net/aspose.cells/horizontalpagebreakcollection/
is_root: false
---
##  HorizontalPageBreakCollection classe
Encapsule une collection de [HorizontalPageBreak](/cells/fr/python-net/aspose.cells/horizontalpagebreak) objets.



Le type HorizontalPageBreakCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableaux peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(row, start_column, end_column)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int-int) | Ajoute un saut de page horizontal à la collection.|
| [add(row)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/add/#int) | Ajoute un saut de page horizontal à la collection.|
| [add(row, column)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int) | Ajoute un saut de page horizontal à la collection.|
| [add(cell_name)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/add/#str) | Ajoute un saut de page horizontal à la collection.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells/horizontalpagebreakcollection/binary_search/#HorizontalPageBreak) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemples

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Voir également
* module [aspose.cells](..)
* classe [HorizontalPageBreak](/cells/fr/python-net/aspose.cells/horizontalpagebreak)
