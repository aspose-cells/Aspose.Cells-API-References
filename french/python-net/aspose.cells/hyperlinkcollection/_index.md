---
title: HyperlinkCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 800
url: /fr/python-net/aspose.cells/hyperlinkcollection/
is_root: false
---
##  HyperlinkCollection classe
Encapsule une collection de [Hyperlink](/cells/fr/python-net/aspose.cells/hyperlink) objets.



Le type HyperlinkCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells/hyperlinkcollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(first_row, first_column, total_rows, total_columns, address)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/add/#int-int-int-int-str) | Ajoute un lien hypertexte à une cellule spécifiée ou à une plage de cellules.|
| [add(cell_name, total_rows, total_columns, address)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/add/#str-int-int-str) | Ajoute un lien hypertexte à une cellule spécifiée ou à une plage de cellules.|
| [add(start_cell_name, end_cell_name, address, text_to_display, screen_tip)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/add/#str-str-str-str-str) | Ajoute un lien hypertexte à une cellule spécifiée ou à une plage de cellules.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells/hyperlinkcollection/binary_search/#Hyperlink) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Get Hyperlinks Collection
hyperlinks = worksheet.hyperlinks
# Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Saving the Excel file
workbook.save("book1.xls")

```

###  Voir également
* module [aspose.cells](..)
* classe [Hyperlink](/cells/fr/python-net/aspose.cells/hyperlink)
