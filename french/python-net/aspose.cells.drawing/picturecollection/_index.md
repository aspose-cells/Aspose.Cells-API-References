---
title: PictureCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 460
url: /fr/python-net/aspose.cells.drawing/picturecollection/
is_root: false
---
##  PictureCollection classe
Encapsule une collection de [Picture](/cells/fr/python-net/aspose.cells.drawing/picture) objets.



Le type PictureCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.drawing/picturecollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableaux peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) | Ajoute une image à la collection.|
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) | Ajoute une image à la collection.|
| [add(upper_left_row, upper_left_column, stream)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) | Ajoute une image à la collection.|
| [add(upper_left_row, upper_left_column, file_name)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) | Ajoute une image à la collection.|
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) | Ajoute une image à la collection.|
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) | Ajoute une image à la collection.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemples

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get PictureCollection
pictures = workbook.worksheets[0].pictures
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Voir également
* module [aspose.cells.drawing](..)
* classe [Picture](/cells/fr/python-net/aspose.cells.drawing/picture)
