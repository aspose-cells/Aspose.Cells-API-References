---
title: set_dynamic_array_formula méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 310
url: /fr/python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---
##  set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}
Définit la formule de tableau dynamique et fait en sorte que la formule se répande dans les cellules voisines si possible.


###  Retour

la plage dans laquelle la formule doit déborder.


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| array_formula | str | l'expression de la formule|
| options | [FormulaParseOptions](/cells/fr/python-net/aspose.cells/formulaparseoptions) | options pour analyser la formule.<br/> L'option "Parser" sera ignorée et la formule sera toujours analysée immédiatement|
| calculate_value | bool | si calculer cette formule de tableau dynamique pour les cellules de la plage renversée.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}
Définit la formule de tableau dynamique et fait en sorte que la formule se répande dans les cellules voisines si possible.


###  Retour

la plage dans laquelle la formule doit déborder.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| array_formula | str | l'expression de la formule|
| options | [FormulaParseOptions](/cells/fr/python-net/aspose.cells/formulaparseoptions) | options pour analyser la formule.<br/> L'option "Parser" sera ignorée et la formule sera toujours analysée immédiatement|
| values | list |valeurs pour ces cellules avec une formule de tableau dynamique donnée|
| calculate_range | bool | Calcule ou non la plage déversée pour cette formule de tableau dynamique.<br/>Si le paramètre "values" n'est pas nul et que ce drapeau est faux,<br/>alors la hauteur de la plage renversée sera values.Length et width seront values[0].Length.|
| calculate_value | bool | si calculer cette formule de tableau dynamique pour les cellules de la plage renversée lorsque "values" est null<br/> ou l'élément correspondant dans "valeurs" pour une cellule est nul.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}
Définit la formule de tableau dynamique et fait en sorte que la formule se répande dans les cellules voisines si possible.


###  Retour

la plage dans laquelle la formule doit déborder.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| array_formula | str | l'expression de la formule|
| options | [FormulaParseOptions](/cells/fr/python-net/aspose.cells/formulaparseoptions) | options pour analyser la formule.<br/> L'option "Parser" sera ignorée et la formule sera toujours analysée immédiatement|
| values | list |valeurs pour ces cellules avec une formule de tableau dynamique donnée|
| calculate_range | bool | Calcule ou non la plage déversée pour cette formule de tableau dynamique.<br/>Si le paramètre "values" n'est pas nul et que ce drapeau est faux,<br/>alors la hauteur de la plage renversée sera values.Length et width seront values[0].Length.|
| calculate_value | bool | si calculer cette formule de tableau dynamique pour les cellules de la plage renversée lorsque "values" est null<br/> ou l'élément correspondant dans "valeurs" pour une cellule est nul.|
| copts | [CalculationOptions](/cells/fr/python-net/aspose.cells/calculationoptions) | Les options de formule de calcul.<br/> Généralement, pour des raisons de performances, la propriété [CalculationOptions.recursive](/cells/fr/python-net/aspose.cells/calculationoptions#recursive) doit être fausse.|



###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
