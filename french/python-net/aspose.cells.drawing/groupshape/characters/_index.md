---
title: characters méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 50
url: /fr/python-net/aspose.cells.drawing/groupshape/characters/
is_root: false
---
##  characters(start_index, length) {#int-int}
Renvoie un objet Characters qui représente une plage de characters dans le texte.


###  Retour

Objet personnages.


```python
def characters(self, start_index, length):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| start_index | int | L'index du début du caractère.|
| length | int | Le nombre de caractères.|
###  Remarques

Cette méthode ne fonctionne que sur la forme avec titre.
###  Exemple


```python

fontSetting = shape.characters(0, 4)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [GroupShape](/cells/fr/python-net/aspose.cells.drawing/groupshape)
