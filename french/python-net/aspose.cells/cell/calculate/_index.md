---
title: calculate méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/cell/calculate/
is_root: false
---
##  calculate(options) {#CalculationOptions}
Calcule la formule de la cellule.



```python
def calculate(self, options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| options | [CalculationOptions](/cells/fr/python-net/aspose.cells/calculationoptions) | Options de calcul|


##  calculate(ignore_error, custom_function) {#bool-ICustomFunction}
Calcule la formule de la cellule.



```python
def calculate(self, ignore_error, custom_function):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| ignore_error | bool | Indique si masquer l'erreur dans le calcul des formules.<br/> L'erreur peut être une fonction non prise en charge, des liens externes, etc.|
| custom_function | [ICustomFunction](/cells/fr/python-net/aspose.cells/icustomfunction) | Les fonctions de calcul de formule personnalisée pour étendre le moteur de calcul.|
###  Remarques

REMARQUE : ce membre est désormais obsolète. Plutôt,
veuillez utiliser la méthode Calculate(CalculationOptions).
 Cette méthode sera supprimée 12 mois plus tard depuis août 2020.
Aspose s'excuse pour tout inconvénient que vous pourriez avoir rencontré.


###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
