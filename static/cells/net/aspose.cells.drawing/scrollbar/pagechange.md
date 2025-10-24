##ScrollBar.PageChange
ScrollBar property. Gets or sets page change
## ScrollBar.PageChange property
Gets or sets page change
```csharp
public int PageChange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ScrollBarPropertyPageChangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a scroll bar to the worksheet
ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
// Set scroll bar properties
scrollBar.Min = 0;
scrollBar.Max = 100;
scrollBar.CurrentValue = 50;
scrollBar.IncrementalChange = 1;
scrollBar.PageChange = 10; // Demonstrate PageChange property
scrollBar.LinkedCell = "A1";
// Save the workbook
workbook.Save("ScrollBarPropertyPageChangeDemo.xlsx");
// Load the saved workbook to verify properties
Workbook verifyWorkbook = new Workbook("ScrollBarPropertyPageChangeDemo.xlsx");
ScrollBar verifyScrollBar = (ScrollBar)verifyWorkbook.Worksheets[0].Shapes[0];
// Output the PageChange property value to demonstrate it was saved/loaded correctly
Console.WriteLine("ScrollBar PageChange value: " + verifyScrollBar.PageChange);
}
}
}
```
### See Also
* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
