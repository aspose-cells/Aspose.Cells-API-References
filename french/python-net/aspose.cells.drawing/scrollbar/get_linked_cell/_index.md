---
title: get_linked_cell méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 100
url: /fr/python-net/aspose.cells.drawing/scrollbar/get_linked_cell/
is_root: false
---
##  get_linked_cell(is_r1c1, is_local) {#bool-bool}
Obtient la plage liée à la valeur du contrôle.


###  Retour

La plage liée à la valeur du contrôle.


```python
def get_linked_cell(self, is_r1c1, is_local):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| is_r1c1 | bool | Indique si la formule doit être formatée en tant que R1C1.|
| is_local | bool | Indique si la formule doit être formatée par les paramètres régionaux.|

###  Exemples

```python

# You may get results like '$A$1'
link = shape.get_linked_cell(False, False)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ScrollBar](/cells/fr/python-net/aspose.cells.drawing/scrollbar)
