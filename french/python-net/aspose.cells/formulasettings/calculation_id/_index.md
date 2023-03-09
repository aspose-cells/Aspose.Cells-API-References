---
title: calculation_id propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 50
url: /fr/python-net/aspose.cells/formulasettings/calculation_id/
is_root: false
---
##  calculation_id propriété

Spécifie la version du moteur de calcul utilisé pour calculer les valeurs dans le classeur.

###  Remarques

Cette propriété sert uniquement à enregistrer les paramètres dans le fichier de feuille de calcul résultant
afin que d'autres applications (telles que ms excel) puissent agir en conséquence lors du chargement et de la manipulation du fichier résultant.
Dans le cas de ms excel, si la valeur de cette propriété est inférieure à l'identifiant du moteur de recalcul associé
avec l'application qui ouvre le fichier résultant, l'application recalculera les résultats de toutes les formules
sur ce classeur immédiatement après le chargement du fichier.
Pour des raisons de performances pour la plupart des applications des utilisateurs, nous ne calculons aucune formule automatiquement sur le classeur,
quelle que soit la valeur définie pour cette propriété.
###  Définition:
```python
@property
def calculation_id(self):
    ...
@calculation_id.setter
def calculation_id(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [FormulaSettings](/cells/fr/python-net/aspose.cells/formulasettings)
