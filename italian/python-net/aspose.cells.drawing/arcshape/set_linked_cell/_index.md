---
title: metodo set_linked_cell
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 180
url: /it/python-net/aspose.cells.drawing/arcshape/set_linked_cell/
is_root: false
---
##  set_linked_cell(formula, is_r1c1, is_local) {#str-bool-bool}
Imposta l'intervallo collegato al valore del controllo.



```python
def set_linked_cell(self, formula, is_r1c1, is_local):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| formula | str | L'intervallo collegato al valore del controllo.|
| is_r1c1 | bool | Se la formula deve essere formattata come R1C1.|
| is_local | bool | Se la formula deve essere formattata in base alle impostazioni locali.|

###  Esempio

```python

# After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
# ActiveX Controls
# Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
# Form Controls
scrollBar = book.worksheets[0].shapes.add_scroll_bar(2, 0, 2, 0, 130, 30)
# Sets the range linked to the control's value.
scrollBar.set_linked_cell("$A$12", False, True)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ArcShape](/cells/it/python-net/aspose.cells.drawing/arcshape)
