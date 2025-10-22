##set_linked_cell method
## set_linked_cell(self, formula, is_r1c1, is_local) {#System.String-bool-bool}
Sets the range linked to the control's value.
```python
def set_linked_cell(self, formula, is_r1c1, is_local):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| formula | System.String | The range linked to the control's value. |
| is_r1c1 | bool | Whether the formula needs to be formatted as R1C1. |
| is_local | bool | Whether the formula needs to be formatted by locale. |
### Example
```python
# After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
# ActiveX Controls
# Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
# Form Controls
scrollBar = book.worksheets[0].shapes.add_scroll_bar(2, 0, 2, 0, 130, 30)
# Sets the range linked to the control's value.
scrollBar.set_linked_cell("$A$12", False, True)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Button`](/cells/python-net/aspose.cells.drawing/button)
