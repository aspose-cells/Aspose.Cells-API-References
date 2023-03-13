---
title: DataSorter classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 420
url: /fr/python-net/aspose.cells/datasorter/
is_root: false
---
##  DataSorter classe
Description sommaire pour DataSorter.



Le type DataSorter expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [keys](/cells/fr/python-net/aspose.cells/datasorter/keys) | Obtient la liste des clés du trieur de données.|
| [has_headers](/cells/fr/python-net/aspose.cells/datasorter/has_headers) | Représente si la plage a des en-têtes.|
| [key1](/cells/fr/python-net/aspose.cells/datasorter/key1) | Représente le premier index de colonne trié (position absolue, la colonne A est 0, B est 1, ...).|
| [order1](/cells/fr/python-net/aspose.cells/datasorter/order1) | Représente l'ordre de tri de la première clé.|
| [key2](/cells/fr/python-net/aspose.cells/datasorter/key2) | Représente l'index de la deuxième colonne triée (position absolue, la colonne A est 0, B est 1, ...).|
| [order2](/cells/fr/python-net/aspose.cells/datasorter/order2) | Représente l'ordre de tri de la deuxième clé.|
| [key3](/cells/fr/python-net/aspose.cells/datasorter/key3) | Représente le troisième index de colonne trié (position absolue, la colonne A est 0, B est 1, ...).|
| [order3](/cells/fr/python-net/aspose.cells/datasorter/order3) | Représente l'ordre de tri de la troisième clé.|
| [sort_left_to_right](/cells/fr/python-net/aspose.cells/datasorter/sort_left_to_right) | True signifie que l'orientation du tri est de gauche à droite.<br/>False signifie que l'orientation du tri est de haut en bas.<br/> La valeur par défaut est faux.|
| [case_sensitive](/cells/fr/python-net/aspose.cells/datasorter/case_sensitive) | Obtient et définit si la casse est sensible lors de la comparaison de chaîne.|
| [sort_as_number](/cells/fr/python-net/aspose.cells/datasorter/sort_as_number) | Indique s'il faut trier tout ce qui ressemble à un nombre.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add_key(key, order)](/cells/fr/python-net/aspose.cells/datasorter/add_key/#int-SortOrder) | Ajoute un index de colonne trié et un ordre de tri.|
| [add_key(key, order, custom_list)](/cells/fr/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-str) | Ajoute un index de colonne trié et un ordre de tri avec une liste de tri personnalisée.|
| [add_key(key, type, order, custom_list)](/cells/fr/python-net/aspose.cells/datasorter/add_key/#int-SortOnType-SortOrder-any) | Ajoute un index de colonne trié et un ordre de tri avec une liste de tri personnalisée.|
| [add_key(key, order, custom_list)](/cells/fr/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-list) | Ajoute un index de colonne trié et un ordre de tri avec une liste de tri personnalisée.|
| [sort(cells, start_row, start_column, end_row, end_column)](/cells/fr/python-net/aspose.cells/datasorter/sort/#Cells-int-int-int-int) | Trie les données de la zone.|
| [sort(cells, area)](/cells/fr/python-net/aspose.cells/datasorter/sort/#Cells-CellArea) | Trier les données de la zone.|
| [sort()](/cells/fr/python-net/aspose.cells/datasorter/sort/#) | Triez les données dans la plage.|
| [clear()](/cells/fr/python-net/aspose.cells/datasorter/clear/#) | Effacez tous les paramètres.|



###  Exemple

```python
from aspose.cells import CellArea, SortOrder, Workbook

# Instantiate a new Workbook object.
workbook = Workbook("Book1.xls")
# Get the workbook datasorter object.
sorter = workbook.data_sorter
# Set the first order for datasorter object.
sorter.order1 = SortOrder.DESCENDING
# Define the first key.
sorter.key1 = 0
# Set the second order for datasorter object.
sorter.order2 = SortOrder.ASCENDING
# Define the second key.
sorter.key2 = 1
# Create a cells area (range).
ca = CellArea()
# Specify the start row index.
ca.start_row = 0
# Specify the start column index.
ca.start_column = 0
# Specify the last row index.
ca.end_row = 13
# Specify the last column index.
ca.end_column = 1
# Sort data in the specified data range (A1:B14)
sorter.sort(workbook.worksheets[0].cells, ca)
# Save the excel file.
workbook.save("outBook.xls")

```

###  Voir également
* module [aspose.cells](..)
