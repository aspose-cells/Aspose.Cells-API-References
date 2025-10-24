##ScrollBar.Min
ScrollBar property. Gets or sets the minimum value of a scroll bar or spinner range
## ScrollBar.Min property
Gets or sets the minimum value of a scroll bar or spinner range.
```csharp
public int Min { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ScrollBarPropertyMinDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a scroll bar to the worksheet
Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
// Set scroll bar properties
scrollBar.Min = 10;
scrollBar.Max = 100;
scrollBar.CurrentValue = 50;  // Changed from Value to CurrentValue
scrollBar.IncrementalChange = 5;
scrollBar.PageChange = 20;
// Display the Min property value
Console.WriteLine("ScrollBar Min Value: " + scrollBar.Min);
// Save the workbook
workbook.Save("ScrollBarMinDemo.xlsx");
}
}
}
```
### See Also
* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
