---
title: invariant_custom propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 260
url: /fr/python-net/aspose.cells/style/invariant_custom/
is_root: false
---
##  invariant_custom propriété

Obtient la chaîne de modèle indépendante de la culture pour le format numérique.
Si aucun format de nombre n'a été défini pour cet objet, null sera renvoyé.
Si le format de nombre est intégré, la chaîne de modèle correspondant au nombre intégré sera renvoyée.

###  Remarques

Pour les formats numériques intégrés, le contenu du modèle renvoyé dépend toujours de la culture,
par exemple, pour certains paramètres régionaux, il renvoie "m/d/y" et pour d'autres paramètres régionaux, il renvoie "d/m/y".
La différence avec [Style.culture_custom](/cells/fr/python-net/aspose.cells/style#culture_custom) est (c'est aussi ce que signifie indépendant de la culture):
les spécificateurs de format et les séparateurs sont conservés en standard, tels que '/' sera toujours utilisé comme séparateur datetime
et "y" sera toujours utilisé comme partie "année", quel que soit l'autre caractère spécial utilisé pour les paramètres régionaux spécifiques.
###  Définition:
```python
@property
def invariant_custom(self):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [Style](/cells/fr/python-net/aspose.cells/style)
