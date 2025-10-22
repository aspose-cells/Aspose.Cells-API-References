##Shape.SetInputRange
Shape method. Sets the range used to fill the control
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
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ShapeMethodSetInputRangeWithStringBooleanBooleanDemo
{
public static void Run()
{
// Create a workbook object
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells A1:A10
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].Value = i + 1;
}
// Add a list box shape
Aspose.Cells.Drawing.Shape listBox = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);
// Set input range for the list box (using String, Boolean, Boolean parameters)
listBox.SetInputRange("$A$1:$A$6", false, false);
// Set linked cell for the list box
listBox.SetLinkedCell("$A$12", false, true);
// Save the workbook
workbook.Save("SetInputRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
