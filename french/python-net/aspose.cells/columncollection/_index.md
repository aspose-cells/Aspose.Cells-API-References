---
title: ColumnCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 270
url: /fr/python-net/aspose.cells/columncollection/
is_root: false
---
##  ColumnCollection classe
Collection des objets [Column](/cells/fr/python-net/aspose.cells/column) qui représentent les colonnes (paramètres) individuelles dans une feuille de calcul.
L'objet Column représente uniquement les paramètres tels que la largeur de colonne, les styles, etc. pour toute la colonne,
n'a rien à voir avec le fait qu'il y ait des cellules (données) non vides ou non dans la colonne correspondante.
Et le "Count" de cette collection ne représente que le nombre d'objets Column qui ont été instanciés dans cette collection,
n'a rien à voir avec le fait qu'il y ait des cellules (données) non vides ou non dans la feuille de calcul.



Le type ColumnCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells/columncollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [copy_to(array)](/cells/fr/python-net/aspose.cells/columncollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells/columncollection/copy_to/#int-list-int-int) | Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells/columncollection/index_of/#Column-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells/columncollection/index_of/#Column-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells/columncollection/last_index_of/#Column) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells/columncollection/last_index_of/#Column-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells/columncollection/last_index_of/#Column-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [get_by_index(index)](/cells/fr/python-net/aspose.cells/columncollection/get_by_index/#int) | Obtient l'objet colonne par l'index.|
| [get_column_by_index(index)](/cells/fr/python-net/aspose.cells/columncollection/get_column_by_index/#int) | Obtient l'objet [Column](/cells/fr/python-net/aspose.cells/column) par la position dans la liste.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells/columncollection/binary_search/#Column) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Add new Style to Workbook
style = workbook.create_style()
# Setting the background color to Blue
style.foreground_color = Color.blue
# setting Background Pattern
style.pattern = BackgroundType.SOLID
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Change the default width of first ten columns
for i in range(10):
    worksheet.cells.columns[i].width = 20
# Get the Column with non default formatting
columns = worksheet.cells.columns
for column in columns:
    # Apply Style to first ten Columns
    column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Voir également
* module [aspose.cells](..)
* classe [Column](/cells/fr/python-net/aspose.cells/column)
