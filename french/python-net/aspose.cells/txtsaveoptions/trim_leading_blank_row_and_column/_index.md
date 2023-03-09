---
title: trim_leading_blank_row_and_column propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 220
url: /fr/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column/
is_root: false
---
##  trim_leading_blank_row_and_column propriété

Indique si les premières lignes et colonnes vides doivent être coupées comme ce que fait MS Excel.
La valeur par défaut est true.

###  Remarques

Même avec la règle dans ms excel, une ligne/colonne ne sera pas considérée comme vide si elle a un style personnalisé,
même s'il ne contient aucune donnée de cellule.
Lors de l'enregistrement en mode LightCells, cette option n'a aucun effet.
L'utilisateur doit contrôler la plage de sortie par la mise en œuvre de [TxtSaveOptions.light_cells_data_provider](/cells/fr/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider)
ou en précisant [TxtSaveOptions.export_area](/cells/fr/python-net/aspose.cells/txtsaveoptions#export_area)
###  Définition:
```python
@property
def trim_leading_blank_row_and_column(self):
    ...
@trim_leading_blank_row_and_column.setter
def trim_leading_blank_row_and_column(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [TxtSaveOptions](/cells/fr/python-net/aspose.cells/txtsaveoptions)
