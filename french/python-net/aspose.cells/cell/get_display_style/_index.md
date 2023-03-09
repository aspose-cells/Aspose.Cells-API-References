---
title: get_display_style méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 110
url: /fr/python-net/aspose.cells/cell/get_display_style/
is_root: false
---
##  get_display_style() {#}
Obtient le style d'affichage de la cellule.
Si cette cellule est également affectée par d'autres paramètres tels que la mise en forme conditionnelle, les objets de liste, etc.,
alors le style d'affichage peut être différent de cell.GetStyle().



```python
def get_display_style(self):
    ...
```




##  get_display_style(include_merged_borders) {#bool}
Obtient le style d'affichage de la cellule.
Si la cellule est au format conditionnel, le style d'affichage n'est pas le même que celui de cell.GetStyle().



```python
def get_display_style(self, include_merged_borders):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| include_merged_borders | bool | Indique s'il faut vérifier les bordures des cellules fusionnées.|



###  Voir également
* module [aspose.cells](../../)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
