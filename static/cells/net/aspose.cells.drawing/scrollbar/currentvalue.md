##ScrollBar.CurrentValue
ScrollBar property. Gets or sets the current value
## ScrollBar.CurrentValue property
Gets or sets the current value.
```csharp
public int CurrentValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ScrollBarPropertyCurrentValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a scroll bar to the worksheet
Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
// Set scroll bar properties using the correct property names
scrollBar.Min = 0;
scrollBar.Max = 100;
scrollBar.IncrementalChange = 5;
scrollBar.PageChange = 20;
// Set and demonstrate CurrentValue property
scrollBar.CurrentValue = 50;
Console.WriteLine("ScrollBar CurrentValue: " + scrollBar.CurrentValue);
// Change the current value
scrollBar.CurrentValue = 75;
Console.WriteLine("Updated ScrollBar CurrentValue: " + scrollBar.CurrentValue);
// Save the workbook
workbook.Save("ScrollBarCurrentValueDemo.xlsx");
}
}
}
```
### See Also
* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
