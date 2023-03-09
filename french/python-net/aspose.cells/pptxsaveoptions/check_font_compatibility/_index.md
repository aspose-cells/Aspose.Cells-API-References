---
title: check_font_compatibility propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 50
url: /fr/python-net/aspose.cells/pptxsaveoptions/check_font_compatibility/
is_root: false
---
##  check_font_compatibility propriété

Indique s'il faut vérifier la compatibilité des polices pour chaque caractère du texte.

###  Remarques

La valeur par défaut est true.
Désactiver cette propriété peut donner de meilleures performances.
Mais lorsque la police par défaut ou spécifiée du texte/caractère ne peut pas être utilisée pour le rendre,
des caractères illisibles (tels que bloc) peuvent apparaître dans le pdf généré.
Pour une telle situation, l'utilisateur doit conserver cette propriété comme vraie afin que
une police alternative peut être recherchée et utilisée pour rendre le texte à la place ;
###  Définition:
```python
@property
def check_font_compatibility(self):
    ...
@check_font_compatibility.setter
def check_font_compatibility(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [PptxSaveOptions](/cells/fr/python-net/aspose.cells/pptxsaveoptions)
