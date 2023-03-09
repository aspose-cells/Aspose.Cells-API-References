---
title: enable_calculation_chain propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 70
url: /fr/python-net/aspose.cells/formulasettings/enable_calculation_chain/
is_root: false
---
##  enable_calculation_chain propriété

Activer ou non la chaîne de calcul pour les formules. La valeur par défaut est false.

###  Remarques

Lorsqu'il y a beaucoup de formules dans le classeur et que l'utilisateur doit les calculer à plusieurs reprises
en n'en modifiant qu'une petite partie, il peut être utile pour les performances d'activer la chaîne de calcul.
D'autre part, si la chaîne est activée, le maintien du modèle de chaîne nécessite de la mémoire supplémentaire,
et cela nécessite également un peu plus de temps processeur pour certaines autres opérations telles que la modification de la valeur ou des formules de la cellule.
Après avoir changé cette propriété de faux à vrai, la chaîne de calcul sera analysée et construite
au moment du premier calcul pour le classeur, donc le temps requis pour le premier calcul
peut être plus que le calcul normal sans chaîne.
###  Définition:
```python
@property
def enable_calculation_chain(self):
    ...
@enable_calculation_chain.setter
def enable_calculation_chain(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [FormulaSettings](/cells/fr/python-net/aspose.cells/formulasettings)
