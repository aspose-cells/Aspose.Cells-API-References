---
title: get_style_in_pool méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 190
url: /fr/python-net/aspose.cells/workbook/get_style_in_pool/
is_root: false
---
##  get_style_in_pool(index) {#int}
Obtient le style dans le pool de styles.
Tous les styles du classeur seront rassemblés dans un pool.
Il n'y a qu'un simple index de référence dans les cellules.


###  Retour

Le style dans le pool correspond à l'index donné, peut être nul.


```python
def get_style_in_pool(self, index):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| index | int | L'index.|
###  Remarques

Si le style renvoyé est modifié, le style de toutes les cellules (qui fait référence à ce style) sera modifié.


###  Voir également

* module [aspose.cells](../../)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
