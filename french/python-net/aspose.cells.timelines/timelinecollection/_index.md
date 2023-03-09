---
title: TimelineCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells.timelines/timelinecollection/
is_root: false
---
##  TimelineCollection classe
Spécifie la collection de tous les objets Timeline sur la feuille de calcul spécifiée.
En raison de MS Excel, Excel 2003 ne prend pas en charge la chronologie.



Le type TimelineCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(pivot, row, column, base_field_name)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-str) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données|
| [add(pivot, dest_cell_name, base_field_name)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-str) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données|
| [add(pivot, row, column, base_field_index)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-int) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données|
| [add(pivot, dest_cell_name, base_field_index)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-int) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données|
| [add(pivot, row, column, base_field)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données|
| [add(pivot, dest_cell_name, base_field)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField) | Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données|
| [copy_to(array)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/copy_to/#int-list-int-int) | Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.timelines/timelinecollection/binary_search/#Timeline) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import CellsFactory, Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
import datetime

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
# Create date style
dateStyle = CellsFactory().create_style()
dateStyle.custom = "m/d/yyyy"
cells.get(0, 1).value = "date"
cells.get(1, 1).value = datetime(2021, 2, 5)
cells.get(2, 1).value = datetime(2022, 3, 8)
cells.get(3, 1).value = datetime(2023, 4, 10)
cells.get(4, 1).value = datetime(2024, 5, 16)
# Set date style
cells.get(1, 1).set_style(dateStyle)
cells.get(2, 1).set_style(dateStyle)
cells.get(3, 1).set_style(dateStyle)
cells.get(4, 1).set_style(dateStyle)
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
pivots = sheet.pivot_tables
# Add a PivotTable
pivotIndex = pivots.add("=Sheet1!A1:C5", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "date")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Refresh PivotTable data
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Voir également
* module [aspose.cells.timelines](..)
