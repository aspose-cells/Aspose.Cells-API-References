---
title: is_param_literal_required propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required/
is_root: false
---
##  is_param_literal_required propriété

Indique si ce moteur a besoin du texte littéral du paramètre lors du calcul. La valeur par défaut est false.

###  Remarques

Si ce moteur de calcul personnalisé nécessite le texte littéral du paramètre, davantage de piles seront nécessaires pour mettre en cache le texte littéral des paramètres et la méthode Calculate() peut être appelée de manière récursive pour calculer la valeur du paramètre.
Généralement, le texte littéral n'est pas nécessaire pour calculer les formules et cette méthode doit renvoyer false pour la plupart des implémentations afin d'obtenir de meilleures performances.
###  Définition:
```python
@property
def is_param_literal_required(self):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [AbstractCalculationEngine](/cells/fr/python-net/aspose.cells/abstractcalculationengine)
