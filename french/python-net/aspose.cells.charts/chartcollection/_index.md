---
title: ChartCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 50
url: /fr/python-net/aspose.cells.charts/chartcollection/
is_root: false
---
##  ChartCollection classe
Encapsule une collection de [Chart](/cells/fr/python-net/aspose.cells.charts/chart) objets.



Le type ChartCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.charts/chartcollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableaux peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/fr/python-net/aspose.cells.charts/chartcollection/add/#ChartType-int-int-int-int) | Ajoute un graphique à la collection.|
| [add(type, data_range, top_row, left_column, right_row, bottom_column)](/cells/fr/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-int-int-int-int) | Ajoute un graphique à la collection.|
| [add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/fr/python-net/aspose.cells.charts/chartcollection/add/#bytes-str-bool-int-int-int-int) | Ajoute un graphique avec un modèle prédéfini.|
| [add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/fr/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-bool-int-int-int-int) | Ajoute un graphique à la collection.|
| [get(index)](/cells/fr/python-net/aspose.cells.charts/chartcollection/get/#int) |Ajouter API for Python Via .Net.car cet [int index] n'est pas pris en charge|
| [get(name)](/cells/fr/python-net/aspose.cells.charts/chartcollection/get/#str) | Ajouter API for Python Via .Net.car ce [chaîne de caractères] n'est pas pris en charge|
| [copy_to(array)](/cells/fr/python-net/aspose.cells.charts/chartcollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.charts/chartcollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [add_floating_chart(type, left, top, width, height)](/cells/fr/python-net/aspose.cells.charts/chartcollection/add_floating_chart/#ChartType-int-int-int-int) | Ajoute un graphique à la collection.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.charts/chartcollection/binary_search/#Chart) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemples

```python
from aspose.cells import Workbook

workbook = Workbook()
charts = workbook.worksheets[0].charts

```

###  Voir également
* module [aspose.cells.charts](..)
* classe [Chart](/cells/fr/python-net/aspose.cells.charts/chart)
