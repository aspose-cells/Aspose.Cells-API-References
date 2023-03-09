---
title: calculate_formula méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells/workbook/calculate_formula/
is_root: false
---
##  calculate_formula() {#}
Calcule le résultat de formules.



```python
def calculate_formula(self):
    ...
```


###  Remarques

Pour toutes les formules prises en charge, veuillez consulter la liste sur https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

##  calculate_formula(ignore_error) {#bool}

Calcule le résultat de formules.



```python
def calculate_formula(self, ignore_error):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| ignore_error | bool | Indique si masquer l'erreur dans le calcul des formules. L'erreur peut être une fonction non prise en charge, des liens externes, etc.|


##  calculate_formula(options) {#CalculationOptions}
Calculer des formules dans ce classeur.



```python
def calculate_formula(self, options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| options | [CalculationOptions](/cells/fr/python-net/aspose.cells/calculationoptions) | Options de calcul|


##  calculate_formula(ignore_error, custom_function) {#bool-ICustomFunction}
Calcule le résultat de formules.



```python
def calculate_formula(self, ignore_error, custom_function):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| ignore_error | bool | Indique si masquer l'erreur dans le calcul des formules. L'erreur peut être une fonction non prise en charge, des liens externes, etc.|
| custom_function | [ICustomFunction](/cells/fr/python-net/aspose.cells/icustomfunction) | Les fonctions de calcul de formule personnalisée pour étendre le moteur de calcul.|
###  Remarques

REMARQUE : ce membre est désormais obsolète. Plutôt,
veuillez utiliser la méthode CalculateFormula(CalculationOptions).
 Cette méthode sera supprimée 12 mois plus tard depuis août 2020.
Aspose s'excuse pour tout inconvénient que vous pourriez avoir rencontré.


###  Voir également
* module [aspose.cells](../../)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
