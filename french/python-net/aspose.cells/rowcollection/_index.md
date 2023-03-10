---
title: RowCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1310
url: /fr/python-net/aspose.cells/rowcollection/
is_root: false
---
##  RowCollection classe
Collecte les objets [Row](/cells/fr/python-net/aspose.cells/row) qui représentent les lignes individuelles d'une feuille de calcul.



Le type RowCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [count](/cells/fr/python-net/aspose.cells/rowcollection/count) | Obtient le nombre de lignes dans cette collection.|



Obtient un objet [Row](/cells/fr/python-net/aspose.cells/row) par index de ligne donné. L'objet Row d'un index de ligne donné sera instancié s'il n'existait pas auparavant.
###  Indexeur
| Nom| Description|
| :- | :- |
| [index] |  |


###  Méthodes
| Méthode| Description|
| :- | :- |
| [get_row_by_index(index)](/cells/fr/python-net/aspose.cells/rowcollection/get_row_by_index/#int) | Obtient l'objet de ligne par la position dans la liste.|
| [clear()](/cells/fr/python-net/aspose.cells/rowcollection/clear/#) | Effacer toutes les lignes et cellules.|
| [remove_at(index)](/cells/fr/python-net/aspose.cells/rowcollection/remove_at/#int) | Supprimer la ligne à l'index spécifié|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Get first row
row = worksheet.cells.rows[0]

```

###  Voir également
* module [aspose.cells](..)
* classe [Row](/cells/fr/python-net/aspose.cells/row)
