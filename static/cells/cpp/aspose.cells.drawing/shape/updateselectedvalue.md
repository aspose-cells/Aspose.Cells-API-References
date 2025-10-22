##Aspose::Cells::Drawing::Shape::UpdateSelectedValue method
'Aspose::Cells::Drawing::Shape::UpdateSelectedValue method. Update the selected value by the value of the linked cell in C++.'
## Shape::UpdateSelectedValue method
Update the selected value by the value of the linked cell.
```cpp
void Aspose::Cells::Drawing::Shape::UpdateSelectedValue()
```
## Examples
```cpp
for (int i = 0; i < 10; ++i)
{
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(i, 0);
cell.PutValue(i + 1);
}
//Create a ListBox object
//ActiveX Controls
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);
//Form Controls
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);
//Sets the range used to fill the control.
listBox.SetInputRange(u"$A$1:$A$6", false, false);
//Sets the range linked to the control's value.
listBox.SetLinkedCell(u"$A$12", false, true);
ListBox listbx = (ListBox)listBox;
//Set the value of cell A12
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(11, 0);
cell.PutValue(3);
//Update the selected value by the value of the linked cell.
listBox.UpdateSelectedValue();
//-1 default, no option selected
if (listbx.IsSelected(2))
{
//Option 3 of the ListBox is selected
}
//Change the value of a linked cell
cell.PutValue(4);
//Update the selected value by the value of the linked cell.
listBox.UpdateSelectedValue();
if (listbx.IsSelected(3))
{
//Option 4 of the ListBox is selected
}
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
