---
title: check_excel_restriction propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 70
url: /fr/python-net/aspose.cells/abstracttextloadoptions/check_excel_restriction/
is_root: false
---
##  check_excel_restriction propriété

Si vérifier la restriction du fichier Excel lorsque l'utilisateur modifie les objets liés aux cellules.
Par exemple, Excel n'autorise pas la saisie d'une valeur de chaîne supérieure à 32 Ko.
Lorsque vous saisissez une valeur supérieure à 32 Ko, par exemple Cell.PutValue(string), si cette propriété est vraie, vous obtiendrez une exception.
Si cette propriété est fausse, nous accepterons votre valeur de chaîne d'entrée comme valeur de la cellule afin que plus tard
vous pouvez générer la valeur de chaîne complète pour d'autres formats de fichier tels que CSV.
Cependant, si vous avez défini un type de valeur non valide pour le format de fichier Excel,
vous ne devez pas enregistrer le classeur au format de fichier Excel ultérieurement.
###  Définition:
```python
@property
def check_excel_restriction(self):
    ...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [AbstractTextLoadOptions](/cells/fr/python-net/aspose.cells/abstracttextloadoptions)
