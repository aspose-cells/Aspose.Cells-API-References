---
title: protect méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 180
url: /fr/python-net/aspose.cells/worksheet/protect/
is_root: false
---
##  protect(type) {#ProtectionType}
Protège la feuille de calcul.



```python
def protect(self, type):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| type | [ProtectionType](/cells/fr/python-net/aspose.cells/protectiontype) | Type de protection.|
###  Remarques

Cette méthode protège la feuille de calcul sans mot de passe. Il peut protect feuille de calcul dans toutes les versions du fichier Excel.

##  protect(type, password, old_password) {#ProtectionType-str-str}

Protège la feuille de calcul.



```python
def protect(self, type, password, old_password):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| type | [ProtectionType](/cells/fr/python-net/aspose.cells/protectiontype) | Type de protection.|
| password | str | Mot de passe.|
| old_password | str | Si la feuille de calcul est déjà protégée par un mot de passe, veuillez fournir l'ancien mot de passe.<br/> Sinon, vous pouvez définir une valeur nulle ou une chaîne vide pour ce paramètre.|
###  Remarques

Cette méthode peut protect feuille de calcul dans toutes les versions du fichier Excel.
###  Exemple


```python
from aspose.cells import ProtectionType, Workbook

# Instantiating a Workbook object
excel = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = excel.worksheets[0]
# Protecting the worksheet with a password
worksheet.protect(ProtectionType.ALL, "aspose", None)
# Saving the modified Excel file in default (that is Excel 20003) format
excel.save("output.xls")

```



###  Voir également
* module [aspose.cells](../../)
* classe [Worksheet](/cells/fr/python-net/aspose.cells/worksheet)
