---
title: set_input_range metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 170
url: /sv/python-net/aspose.cells.drawing/oval/set_input_range/
is_root: false
---
##  set_input_range(formula, is_r1c1, is_local) {#str-bool-bool}
Ställer in intervallet som används för att fylla kontrollen.



```python
def set_input_range(self, formula, is_r1c1, is_local):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| formula | str | Området som används för att fylla kontrollen.|
| is_r1c1 | bool | Om formeln behöver formateras som R1C1.|
| is_local | bool | Huruvida formeln behöver formateras efter språk.|

###  Exempel

```python

# After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
# Initialize a new workbook.
# Workbook book = new Workbook();
for i in range(10):
    cell = book.worksheets[0].cells.get(i, 0)
    cell.value = i + 1
# Create a ListBox object
# ActiveX Controls
# Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
# Form Controls
listBox = book.worksheets[0].shapes.add_list_box(2, 0, 2, 0, 130, 130)
# Sets the range used to fill the control.
listBox.set_input_range("$A$1:$A$6", False, False)
# Sets the range linked to the control's value.
listBox.set_linked_cell("$A$12", False, True)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [Oval](/cells/sv/python-net/aspose.cells.drawing/oval)
