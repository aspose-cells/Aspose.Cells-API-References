---
title: get_dependents_in_calculation méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 100
url: /fr/python-net/aspose.cells/cell/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(recursive) {#bool}
Obtient toutes les cellules dont le résultat calculé dépend de cette cellule.


###  Retour

Énumérateur pour énumérer toutes les personnes à charge (objets Cell)


```python
def get_dependents_in_calculation(self, recursive):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| recursive | bool | Si renvoie les personnes à charge qui ne font pas directement référence à cette cellule<br/> mais référence à d'autres feuilles de cette cellule|
###  Remarques

Pour utiliser cette méthode, assurez-vous que le classeur a été défini avec la valeur true pour
[FormulaSettings.enable_calculation_chain](/cells/fr/python-net/aspose.cells/formulasettings#enable_calculation_chain) et a été entièrement calculé avec ce paramètre.
S'il n'y a pas de référence de formule à cette cellule, null sera renvoyé.
###  Exemples

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("B1").get_dependents_in_calculation(False)
print("B1's calculation dependents:")
for c in en:
    print(c.name)
en = cells.get("B2").get_dependents_in_calculation(False)
print("B2's calculation dependents:")
for c in en:
    print(c.name)

```



###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
