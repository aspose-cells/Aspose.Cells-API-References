---
title: get_style méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells/column/get_style/
is_root: false
---
##  get_style() {#}
Obtient le style de cette colonne.



```python
def get_style(self):
    ...
```


###  Remarques

La modification directe de l'objet de style renvoyé n'a aucun effet sur cette colonne ou sur les cellules de cette colonne.
Vous devez appeler la méthode [Column.apply_style(style, flag)](/cells/fr/python-net/aspose.cells/column/apply_style) ou [Column.set_style(style)](/cells/fr/python-net/aspose.cells/column/set_style)
pour appliquer la modification à cette colonne.

Le style de la colonne est le style qui sera hérité par les cellules de cette colonne (les cellules qui n'ont pas de paramètres de style personnalisés,
telles que les cellules existantes dont le style n'a pas été défini explicitement ou celles qui n'ont pas été instanciées)


###  Voir également
* module [aspose.cells](../../)
* classe [Column](/cells/fr/python-net/aspose.cells/column)
