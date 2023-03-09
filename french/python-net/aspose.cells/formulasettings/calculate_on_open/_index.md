---
title: calculate_on_open propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells/formulasettings/calculate_on_open/
is_root: false
---
##  calculate_on_open propriété

Indique si l'application doit effectuer un calcul complet à l'ouverture du classeur.

###  Remarques

Cette propriété sert uniquement à enregistrer les paramètres dans le fichier de feuille de calcul résultant
afin que d'autres applications (telles que ms excel) puissent agir en conséquence lors du chargement du fichier résultant.
Pour des raisons de performances pour la plupart des applications des utilisateurs, nous ne calculons aucune formule automatiquement dans le classeur,
quelle que soit la valeur définie pour cette propriété.
###  Définition:
```python
@property
def calculate_on_open(self):
    ...
@calculate_on_open.setter
def calculate_on_open(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [FormulaSettings](/cells/fr/python-net/aspose.cells/formulasettings)
