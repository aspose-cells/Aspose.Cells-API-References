---
title: CommentCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 290
url: /fr/python-net/aspose.cells/commentcollection/
is_root: false
---
##  CommentCollection classe
Encapsule une collection de [Comment](/cells/fr/python-net/aspose.cells/comment) objets.



Le type CommentCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells/commentcollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add_threaded_comment(row, column, text, author)](/cells/fr/python-net/aspose.cells/commentcollection/add_threaded_comment/#int-int-str-ThreadedCommentAuthor) | Ajoute un commentaire fileté.|
| [add_threaded_comment(cell_name, text, author)](/cells/fr/python-net/aspose.cells/commentcollection/add_threaded_comment/#str-str-ThreadedCommentAuthor) | Ajoute un commentaire fileté.|
| [get_threaded_comments(row, column)](/cells/fr/python-net/aspose.cells/commentcollection/get_threaded_comments/#int-int) | Obtient les commentaires thématiques par index de ligne et de colonne.|
| [get_threaded_comments(cell_name)](/cells/fr/python-net/aspose.cells/commentcollection/get_threaded_comments/#str) | Obtient les commentaires thématiques par nom de cellule.|
| [add(row, column)](/cells/fr/python-net/aspose.cells/commentcollection/add/#int-int) | Ajoute un commentaire à la collection.|
| [add(cell_name)](/cells/fr/python-net/aspose.cells/commentcollection/add/#str) | Ajoute un commentaire à la collection.|
| [remove_at(cell_name)](/cells/fr/python-net/aspose.cells/commentcollection/remove_at/#str) | Supprime le commentaire de la cellule spécifique.|
| [remove_at(row, column)](/cells/fr/python-net/aspose.cells/commentcollection/remove_at/#int-int) | Supprime le commentaire de la cellule spécifique.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells/commentcollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells/commentcollection/copy_to/#int-list-int-int) | Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells/commentcollection/index_of/#Comment-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells/commentcollection/index_of/#Comment-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells/commentcollection/last_index_of/#Comment) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells/commentcollection/binary_search/#Comment) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import Workbook

workbook = Workbook()
comments = workbook.worksheets[0].comments

```

###  Voir également
* module [aspose.cells](..)
* classe [Comment](/cells/fr/python-net/aspose.cells/comment)
