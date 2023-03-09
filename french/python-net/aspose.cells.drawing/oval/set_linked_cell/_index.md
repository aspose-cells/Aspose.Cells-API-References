---
title: set_linked_cell méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 180
url: /fr/python-net/aspose.cells.drawing/oval/set_linked_cell/
is_root: false
---
##  set_linked_cell(formula, is_r1c1, is_local) {#str-bool-bool}
Définit la plage liée à la valeur du contrôle.



```python
def set_linked_cell(self, formula, is_r1c1, is_local):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| formula | str |La plage liée à la valeur du contrôle.|
| is_r1c1 | bool | Indique si la formule doit être formatée en tant que R1C1.|
| is_local | bool | Indique si la formule doit être formatée par les paramètres régionaux.|

###  Exemple

```python

# After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
# ActiveX Controls
# Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
# Form Controls
scrollBar = book.worksheets[0].shapes.add_scroll_bar(2, 0, 2, 0, 130, 30)
# Sets the range linked to the control's value.
scrollBar.set_linked_cell("$A$12", False, True)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [Oval](/cells/fr/python-net/aspose.cells.drawing/oval)
