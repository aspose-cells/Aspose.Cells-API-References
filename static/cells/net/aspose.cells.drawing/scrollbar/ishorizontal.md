##ScrollBar.IsHorizontal
ScrollBar property. Indicates whether this is a horizontal scroll bar
## ScrollBar.IsHorizontal property
Indicates whether this is a horizontal scroll bar.
```csharp
public bool IsHorizontal { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ScrollBarPropertyIsHorizontalDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a horizontal scroll bar
Shape scrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 0, 100, 20);
ScrollBar scrollBar = (ScrollBar)scrollBarShape;
scrollBar.IsHorizontal = true;
// Add a vertical scroll bar for comparison
Shape verticalScrollBarShape = worksheet.Shapes.AddScrollBar(1, 0, 1, 30, 20, 100);
ScrollBar verticalScrollBar = (ScrollBar)verticalScrollBarShape;
verticalScrollBar.IsHorizontal = false;
// Demonstrate IsHorizontal property
Console.WriteLine("Horizontal Scroll Bar IsHorizontal: " + scrollBar.IsHorizontal);
Console.WriteLine("Vertical Scroll Bar IsHorizontal: " + verticalScrollBar.IsHorizontal);
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
