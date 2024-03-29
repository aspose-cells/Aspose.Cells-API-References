---
title: Shape.SetInputRange
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Sets the range used to fill the control
type: docs
url: /net/aspose.cells.drawing/shape/setinputrange/
---
## Shape.SetInputRange method

Sets the range used to fill the control.

```csharp
public void SetInputRange(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The range used to fill the control. |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |

### Examples

```csharp

[C#]
//After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.

for (int i = 0; i< 10; ++i)
{
    Cell cell = book.Worksheets[0].Cells[i, 0];
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

```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


