---
title: pivot_source propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 400
url: /fr/python-net/aspose.cells.charts/chart/pivot_source/
is_root: false
---
##  pivot_source propriété

La source est les données du tableau croisé dynamique.
Si PivotSource n'est pas vide, le graphique est PivotChart.

###  Remarques

Si le tableau croisé dynamique "PivotTable1" dans la feuille de calcul "Sheet1" dans le fichier "Book1.xls".
Le pivotSource peut être "[Book1.xls]Sheet1!PivotTable1" si le graphique et le tableau croisé dynamique ne se trouvent pas dans le même classeur.
Si vous définissez cette propriété, le paramètre de source de données précédent sera perdu.
###  Définition:
```python
@property
def pivot_source(self):
    ...
@pivot_source.setter
def pivot_source(self, value):
    ...
```

###  Voir également
* module [aspose.cells.charts](../../)
* classe [Chart](/cells/fr/python-net/aspose.cells.charts/chart)
