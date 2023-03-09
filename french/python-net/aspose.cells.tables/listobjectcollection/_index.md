---
title: ListObjectCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells.tables/listobjectcollection/
is_root: false
---
##  ListObjectCollection classe
Représente une collection de [ListObject](/cells/fr/python-net/aspose.cells.tables/listobject) objets dans la feuille de calcul.



Le type ListObjectCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(start_row, start_column, end_row, end_column, has_headers)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/add/#int-int-int-int-bool) | Ajoute un ListObject à la feuille de calcul.|
| [add(start_cell, end_cell, has_headers)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/add/#str-str-bool) | Ajoute un ListObject à la feuille de calcul.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/copy_to/#int-list-int-int) | Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/index_of/#ListObject-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/index_of/#ListObject-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/last_index_of/#ListObject) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/last_index_of/#ListObject-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/last_index_of/#ListObject-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [update_column_name()](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/update_column_name/#) | Mettez à jour tous les noms de colonne des tables.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.tables/listobjectcollection/binary_search/#ListObject) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Voir également
* module [aspose.cells.tables](..)
* classe [ListObject](/cells/fr/python-net/aspose.cells.tables/listobject)
