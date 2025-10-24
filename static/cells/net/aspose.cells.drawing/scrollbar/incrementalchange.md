##ScrollBar.IncrementalChange
ScrollBar property. Gets or sets the amount that the scroll bar or spinner is incremented a line scroll
## ScrollBar.IncrementalChange property
Gets or sets the amount that the scroll bar or spinner is incremented a line scroll.
```csharp
public int IncrementalChange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ScrollBarPropertyIncrementalChangeDemo
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
scrollBar.IncrementalChange = 5; // This is the key property we're demonstrating
scrollBar.PageChange = 20;
// Display the scroll bar properties
Console.WriteLine("Scroll Bar Properties:");
Console.WriteLine("Min: " + scrollBar.Min);
Console.WriteLine("Max: " + scrollBar.Max);
Console.WriteLine("Current Value: " + scrollBar.CurrentValue);
Console.WriteLine("Incremental Change: " + scrollBar.IncrementalChange);
Console.WriteLine("Page Change: " + scrollBar.PageChange);
// Modify the incremental change
scrollBar.IncrementalChange = 10;
Console.WriteLine("\nModified Incremental Change: " + scrollBar.IncrementalChange);
// Save the workbook
workbook.Save("ScrollBarDemo.xlsx");
}
}
}
```
### See Also
* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
