---
title: set_formulas méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 60
url: /fr/python-net/aspose.cells/formatcondition/set_formulas/
is_root: false
---
##  set_formulas(formula1, formula2, is_r1c1, is_local) {#str-str-bool-bool}
Définit la valeur ou l'expression associée à cette condition de format.



```python
def set_formulas(self, formula1, formula2, is_r1c1, is_local):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| formula1 | str | La valeur ou l'expression associée à cette condition de format.<br/>Si la valeur d'entrée commence par '=', elle sera considérée comme une formule. Sinon, il sera pris comme valeur simple (texte, nombre, booléen).<br/> Pour une valeur de texte commençant par '=', l'utilisateur peut la saisir sous forme de formule au format : "=\"=...\"".|
| formula2 | str | La valeur ou l'expression associée à cette condition de format. Le format d'entrée est le même avec formula1|
| is_r1c1 | bool | Si la formule est la formule R1C1.|
| is_local | bool | Indique si la formule est formatée en paramètres régionaux.|



###  Voir également
* module [aspose.cells](../../)
* classe [FormatCondition](/cells/fr/python-net/aspose.cells/formatcondition)
