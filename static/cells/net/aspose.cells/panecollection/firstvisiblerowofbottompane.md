##PaneCollection.FirstVisibleRowOfBottomPane
PaneCollection property. Gets and sets the first visible row of the bottom pane
## PaneCollection.FirstVisibleRowOfBottomPane property
Gets and sets the first visible row of the bottom pane.
```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a scrollable pane
for (int i = 0; i < 50; i++)
{
worksheet.Cells[i, 0].Value = "Row " + (i + 1);
}
// Freeze panes at row 10 (this will create top and bottom panes)
worksheet.FreezePanes(10, 0, 10, 0);
// Get the panes collection
PaneCollection panes = worksheet.GetPanes();
// Set the first visible row of the bottom pane
panes.FirstVisibleRowOfBottomPane = 15;
// Output the first visible row of bottom pane
Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
// Save the workbook
workbook.Save("PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo.xlsx");
}
}
}
```
### See Also
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
