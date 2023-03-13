---
title: get_picture méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 120
url: /fr/python-net/aspose.cells/pagesetup/get_picture/
is_root: false
---
##  get_picture(is_header, section) {#bool-int}
Obtient l'objet [Picture](/cells/fr/python-net/aspose.cells.drawing/picture) de l'en-tête/pied de page.


###  Retour

Renvoie l'objet [Picture](/cells/fr/python-net/aspose.cells.drawing/picture).
Renvoie null s'il n'y a pas d'image.


```python
def get_picture(self, is_header, section):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| is_header | bool | Indique s'il se trouve dans l'en-tête ou le pied de page.|
| section | int | 0 : Section gauche, 1 : Section centrale, 2 : Section droite.|


##  get_picture(is_first, is_even, is_header, section) {#bool-bool-bool-int}
Obtient l'objet [Picture](/cells/fr/python-net/aspose.cells.drawing/picture) de l'en-tête/pied de page.


###  Retour

Renvoie l'objet [Picture](/cells/fr/python-net/aspose.cells.drawing/picture).


```python
def get_picture(self, is_first, is_even, is_header, section):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| is_first | bool | Indique si l'image de l'en-tête/du pied de page de la première page est récupérée.|
| is_even | bool | Indique si l'image d'un en-tête/pied de page pair est obtenue.|
| is_header | bool | Indique si l'image de l'en-tête/du pied de page est récupérée.|
| section | int | 0 : Section gauche, 1 : Section centrale, 2 : Section droite.|



###  Voir également
* module [aspose.cells](../../)
* classe [PageSetup](/cells/fr/python-net/aspose.cells/pagesetup)
* classe [Picture](/cells/fr/python-net/aspose.cells.drawing/picture)
