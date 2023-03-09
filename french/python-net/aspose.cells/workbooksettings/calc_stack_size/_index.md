---
title: calc_stack_size propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 100
url: /fr/python-net/aspose.cells/workbooksettings/calc_stack_size/
is_root: false
---
##  calc_stack_size propriété

Spécifie la taille de la pile pour le calcul récursif des cellules.
La valeur élevée de cette taille donnera de meilleures performances lorsque de nombreuses cellules doivent être calculées de manière récursive.
D'autre part, une valeur plus élevée augmentera le risque de StackOverflowException.
Si l'utilisateur obtient StackOverflowException lors du calcul des formules, cette valeur doit être diminuée.

###  Remarques

REMARQUE : ce membre est désormais obsolète. À la place, veuillez utiliser CalculationOptions
avec le CalcStackSize spécifié lors du calcul des formules.
 Cette propriété sera supprimée 12 mois plus tard depuis février 2022.
Aspose s'excuse pour tout inconvénient que vous pourriez avoir rencontré.
###  Définition:
```python
@property
def calc_stack_size(self):
    ...
@calc_stack_size.setter
def calc_stack_size(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [WorkbookSettings](/cells/fr/python-net/aspose.cells/workbooksettings)
