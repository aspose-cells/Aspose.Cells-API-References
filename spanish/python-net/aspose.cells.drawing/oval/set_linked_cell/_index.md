---
title: set_linked_cell método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 180
url: /es/python-net/aspose.cells.drawing/oval/set_linked_cell/
is_root: false
---
##  set_linked_cell(formula, is_r1c1, is_local) {#str-bool-bool}
Establece el rango vinculado al valor del control.



```python
def set_linked_cell(self, formula, is_r1c1, is_local):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| formula | str | El rango vinculado al valor del control.|
| is_r1c1 | bool | Si la fórmula debe formatearse como R1C1.|
| is_local | bool | Si la fórmula debe formatearse según la configuración regional.|

###  Ejemplos

```python

# After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
# ActiveX Controls
# Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
# Form Controls
scrollBar = book.worksheets[0].shapes.add_scroll_bar(2, 0, 2, 0, 130, 30)
# Sets the range linked to the control's value.
scrollBar.set_linked_cell("$A$12", False, True)

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [Oval](/cells/es/python-net/aspose.cells.drawing/oval)
