##Worksheet.GetPanes
Worksheet method. Gets the window panes
## Worksheet.GetPanes method
Gets the window panes.
```csharp
public PaneCollection GetPanes()
```
### Remarks
If the window is not split or frozen.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodGetPanesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Freeze panes at row 5 and column 3
worksheet.FreezePanes(5, 3, 5, 3);
// Get pane information
PaneCollection panes = worksheet.GetPanes();
// Display pane information
Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
Console.WriteLine("First visible column of right pane: " + panes.FirstVisibleColumnOfRightPane);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
