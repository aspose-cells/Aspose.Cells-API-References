---
title: refer_to_sheet_with_same_name propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 90
url: /fr/python-net/aspose.cells/copyoptions/refer_to_sheet_with_same_name/
is_root: false
---
##  refer_to_sheet_with_same_name propriété

Lors de la copie d'une feuille de calcul dans un autre classeur et que la feuille de calcul contient les formules qui font référence à d'autres feuilles de calcul dans MS Excel,
 les formules copiées doivent faire référence au classeur source.
Mais parfois, nous avons copié d'autres feuilles de calcul et nous espérons que les formules copiées font référence à d'autres feuilles de calcul avec le nom dans le même classeur,
veuillez définir cette propriété sur true.

###  Remarques

La valeur par défaut est true.
###  Définition:
```python
@property
def refer_to_sheet_with_same_name(self):
    ...
@refer_to_sheet_with_same_name.setter
def refer_to_sheet_with_same_name(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [CopyOptions](/cells/fr/python-net/aspose.cells/copyoptions)
