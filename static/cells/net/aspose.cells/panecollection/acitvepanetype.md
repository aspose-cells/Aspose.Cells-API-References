##PaneCollection.AcitvePaneType
PaneCollection property. Gets and sets the active pane
## PaneCollection.AcitvePaneType property
Gets and sets the active pane.
```csharp
public RectangleAlignmentType AcitvePaneType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class PaneCollectionPropertyAcitvePaneTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to demonstrate pane splitting
for (int i = 0; i < 20; i++)
{
for (int j = 0; j < 10; j++)
{
worksheet.Cells[i, j].Value = $"Row {i + 1}, Col {j + 1}";
}
}
// Split the worksheet into panes
worksheet.Split();
// Get the pane collection
PaneCollection panes = worksheet.GetPanes();
// Display current active pane
Console.WriteLine("Current ActivePaneType: " + panes.AcitvePaneType);
// Set active pane to BottomRight
panes.AcitvePaneType = RectangleAlignmentType.BottomRight;
Console.WriteLine("Changed ActivePaneType to: " + panes.AcitvePaneType);
// Set first visible row/column for bottom/right panes
panes.FirstVisibleRowOfBottomPane = 15;
panes.FirstVisibleColumnOfRightPane = 7;
// Save the workbook
workbook.Save("PaneCollectionActivePaneTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [RectangleAlignmentType](../../../aspose.cells.drawing/rectanglealignmenttype/)
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
