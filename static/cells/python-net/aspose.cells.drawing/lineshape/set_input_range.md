##set_input_range method
## set_input_range(self, formula, is_r1c1, is_local) {#System.String-bool-bool}
Sets the range used to fill the control.
```python
def set_input_range(self, formula, is_r1c1, is_local):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| formula | System.String | The range used to fill the control. |
| is_r1c1 | bool | Whether the formula needs to be formatted as R1C1. |
| is_local | bool | Whether the formula needs to be formatted by locale. |
### Example
```python
# After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
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
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`LineShape`](/cells/python-net/aspose.cells.drawing/lineshape)
