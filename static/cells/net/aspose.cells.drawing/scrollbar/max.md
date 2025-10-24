##ScrollBar.Max
ScrollBar property. Gets or sets the maximum value of a scroll bar or spinner range
## ScrollBar.Max property
Gets or sets the maximum value of a scroll bar or spinner range.
```csharp
public int Max { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ScrollBarPropertyMaxDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a scroll bar to the worksheet
Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
// Set scroll bar properties
scrollBar.Min = 0;
scrollBar.Max = 100; // Demonstrating Max property usage
scrollBar.CurrentValue = 50;
scrollBar.IncrementalChange = 5;
scrollBar.PageChange = 10;
// Save the workbook
workbook.Save("ScrollBarMaxDemo.xlsx");
// Display info
Console.WriteLine("ScrollBar created with Max value: " + scrollBar.Max.ToString());
Console.WriteLine("File saved successfully.");
}
}
}
```
### See Also
* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
