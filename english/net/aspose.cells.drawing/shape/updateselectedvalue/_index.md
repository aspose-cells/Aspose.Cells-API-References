---
title: Shape.UpdateSelectedValue
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Update the selected value by the value of the linked cell
type: docs
url: /net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

Update the selected value by the value of the linked cell.

```csharp
public void UpdateSelectedValue()
```

### Examples

```csharp

[C#]
Cell cell = null;
for (int i = 0; i< 10; ++i)
{
    cell = book.Worksheets[0].Cells[i, 0];
    cell.Value = i + 1;
}
   
//Create a ListBox object

//ActiveX Controls
//Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);

//Form Controls
Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddListBox(2, 0, 2, 0, 130, 130);

//Sets the range used to fill the control.
listBox.SetInputRange("$A$1:$A$6", false, false);

//Sets the range linked to the control's value.
listBox.SetLinkedCell("$A$12", false, true);

ListBox listbx = (ListBox)listBox;

//Set the value of cell A12
cell = book.Worksheets[0].Cells[11, 0];
cell.Value = 3;

//Update the selected value by the value of the linked cell.
listBox.UpdateSelectedValue();

//-1 default, no option selected
if(listbx.IsSelected(2))
{
    //Option 3 of the ListBox is selected
}

//Change the value of a linked cell
cell.Value = 4;

//Update the selected value by the value of the linked cell.
listBox.UpdateSelectedValue();
if(listbx.IsSelected(3))
{
    //Option 4 of the ListBox is selected
}

```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


