##MsoLineFormat.IsVisible
MsoLineFormat property. Indicates whether the object is visible
## MsoLineFormat.IsVisible property
Indicates whether the object is visible.
```csharp
public bool IsVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MsoLineFormatPropertyIsVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with visible border
var shape1 = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
shape1.LineFormat.IsVisible = true;
// Add an oval shape with invisible border
var shape2 = worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
shape2.LineFormat.IsVisible = false;
// Verify and print the IsVisible property values
Console.WriteLine("Rectangle border visible: " + shape1.LineFormat.IsVisible);
Console.WriteLine("Oval border visible: " + shape2.LineFormat.IsVisible);
// Save the workbook
workbook.Save("MsoLineFormat_IsVisible_Demo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
