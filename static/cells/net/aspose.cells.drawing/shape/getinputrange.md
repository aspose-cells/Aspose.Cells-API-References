##Shape.GetInputRange
Shape method. Gets the range used to fill the control
## Shape.GetInputRange method
Gets the range used to fill the control.
```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
### Return Value
The range used to fill the control.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodGetInputRangeWithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Input 1");
worksheet.Cells["A2"].PutValue("Input 2");
worksheet.Cells["A3"].PutValue("Input 3");
// Add a list box shape
ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 0, 0);
Shape shape = listBox;
// Set the input range for the list box
shape.SetInputRange("$A$1:$A$3", false, false);
// Get the input range
string range = shape.GetInputRange(false, true);
Console.WriteLine("Shape input range: " + range);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
