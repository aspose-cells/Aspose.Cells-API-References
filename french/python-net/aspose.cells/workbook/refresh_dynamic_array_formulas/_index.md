---
title: refresh_dynamic_array_formulas méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 270
url: /fr/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/
is_root: false
---
##  refresh_dynamic_array_formulas(calculate) {#bool}
Actualise les formules de tableau dynamique (débordement dans une nouvelle plage de cellules voisines en fonction des données actuelles)
Les autres formules du classeur ne seront pas calculées de manière récursive même si elles ont été utilisées par des formules matricielles dynamiques.



```python
def refresh_dynamic_array_formulas(self, calculate):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| calculate | bool | Si calcule et met à jour les valeurs des cellules pour ces formules de tableau dynamique|


##  refresh_dynamic_array_formulas(calculate, copts) {#bool-CalculationOptions}
Actualise les formules de tableau dynamique (débordement dans une nouvelle plage de cellules voisines en fonction des données actuelles)



```python
def refresh_dynamic_array_formulas(self, calculate, copts):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| calculate | bool | Si calcule et met à jour les valeurs des cellules pour ces formules de tableau dynamique|
| copts | [CalculationOptions](/cells/fr/python-net/aspose.cells/calculationoptions) | Les options de calcul des formules|



###  Voir également
* module [aspose.cells](../../)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
