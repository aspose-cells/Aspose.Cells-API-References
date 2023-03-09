---
title: trim_tailing_blank_cells propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 230
url: /fr/python-net/aspose.cells/txtsaveoptions/trim_tailing_blank_cells/
is_root: false
---
##  trim_tailing_blank_cells propriété

Indique si les cellules vides de fin d'une ligne doivent être supprimées. La valeur par défaut est false.

###  Remarques

Lors de l'enregistrement avec le mode LightCells et que le [TxtSaveOptions.export_area](/cells/fr/python-net/aspose.cells/txtsaveoptions#export_area) n'a pas été spécifié,
cette option n'a aucun effet et une ligne sera étendue à la dernière cellule fournie par
la mise en œuvre [TxtSaveOptions.light_cells_data_provider](/cells/fr/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider)
###  Définition:
```python
@property
def trim_tailing_blank_cells(self):
    ...
@trim_tailing_blank_cells.setter
def trim_tailing_blank_cells(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [TxtSaveOptions](/cells/fr/python-net/aspose.cells/txtsaveoptions)
