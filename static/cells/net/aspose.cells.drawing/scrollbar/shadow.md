##ScrollBar.Shadow
ScrollBar property. Indicates whether the shape has 3D shading
## ScrollBar.Shadow property
Indicates whether the shape has 3-D shading.
```csharp
public bool Shadow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ScrollBarPropertyShadowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a horizontal scroll bar
ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
// Set scroll bar properties
scrollBar.Min = 0;
scrollBar.Max = 100;
scrollBar.IncrementalChange = 5;
scrollBar.PageChange = 20;
scrollBar.CurrentValue = 50;
scrollBar.IsHorizontal = true;
// Demonstrate Shadow property
scrollBar.Shadow = true; // Enable 3D shadow effect
// Create another scroll bar for comparison
ScrollBar scrollBar2 = worksheet.Shapes.AddScrollBar(1, 2, 1, 1, 100, 20);
scrollBar2.Shadow = false; // No shadow
// Save the workbook
workbook.Save("ScrollBarShadowDemo.xlsx");
Console.WriteLine("ScrollBar Shadow demo completed. Check output file.");
}
}
}
```
### See Also
* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
