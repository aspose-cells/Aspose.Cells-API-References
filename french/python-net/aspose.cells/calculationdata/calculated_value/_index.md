---
title: calculated_value propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 50
url: /fr/python-net/aspose.cells/calculationdata/calculated_value/
is_root: false
---
##  calculated_value propriété

Obtient ou définit la valeur calculée pour cette fonction.

###  Remarques

L'utilisateur doit définir cette propriété dans son moteur de calcul personnalisé pour les fonctions prises en charge par le moteur,
et la valeur définie sera renvoyée lors de l'obtention ultérieure de cette propriété.
La valeur définie peut être n'importe quelle valeur de ces objets pouvant être définie sur Cell(Cell.Value).
Et il peut également s'agir d'un tableau de ce type de valeurs, ou d'un Range, Name, ReferredArea.
L'obtention de cette propriété avant la définition fera que la fonction sera calculée par le moteur de calcul par défaut de Aspose.Cells et la valeur calculée sera renvoyée.
###  Définition:
```python
@property
def calculated_value(self):
    ...
@calculated_value.setter
def calculated_value(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [CalculationData](/cells/fr/python-net/aspose.cells/calculationdata)
