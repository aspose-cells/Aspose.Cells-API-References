---
title: calculation_mode propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 60
url: /fr/python-net/aspose.cells/formulasettings/calculation_mode/
is_root: false
---
##  calculation_mode propriété

Obtient ou définit le mode de calcul du classeur dans MS Excel.

###  Remarques

Cette propriété sert uniquement à enregistrer les paramètres dans le fichier de feuille de calcul résultant
afin que d'autres applications (telles que ms excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant.
Pour des raisons de performances pour la plupart des applications de l'utilisateur, nous ne calculons automatiquement aucune formule dans le classeur,
quel que soit le mode défini pour cette propriété.
Si l'utilisateur a besoin de calculer des formules, veuillez toujours appeler des méthodes sur différents objets en fonction des besoins :
[Workbook.calculate_formula()](/cells/python-net/aspose.cells/workbook/calculate_formula), [Worksheet.calculate_formula(formula)](/cells/python-net/aspose.cells/worksheet/calculate_formula),
[Cell.calculate(options)](/cells/python-net/aspose.cells/cell/calculate), ...etc.
###  Définition:
```python
@property
def calculation_mode(self):
    ...
@calculation_mode.setter
def calculation_mode(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [CalcModeType](/cells/fr/python-net/aspose.cells/calcmodetype)
* classe [FormulaSettings](/cells/fr/python-net/aspose.cells/formulasettings)
