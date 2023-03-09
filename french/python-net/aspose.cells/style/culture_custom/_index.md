---
title: culture_custom propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 170
url: /fr/python-net/aspose.cells/style/culture_custom/
is_root: false
---
##  culture_custom propriété

Obtient et définit la chaîne de modèle dépendante de la culture pour le format numérique.
Si aucun format de nombre n'a été défini pour cet objet, null sera renvoyé.
Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée.

###  Remarques

Pour le format de nombre intégré, à la fois le contenu du modèle (par exemple, un format de date intégré est "m/d/y" pour certains paramètres régionaux,
mais pour certains autres paramètres régionaux, il devient "d/m/y") et le spécificateur de format (tel que,
certains paramètres régionaux utilisent un caractère autre que 'y' pour représenter la partie année pour le formatage de la date)
dépendent de la culture ;
Pour le format personnalisé spécifié par l'utilisateur, seuls les spécificateurs de format sont modifiés en fonction de la culture,
les autres parties du modèle de formatage ne seront pas modifiées.
###  Définition:
```python
@property
def culture_custom(self):
    ...
@culture_custom.setter
def culture_custom(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [Style](/cells/fr/python-net/aspose.cells/style)
