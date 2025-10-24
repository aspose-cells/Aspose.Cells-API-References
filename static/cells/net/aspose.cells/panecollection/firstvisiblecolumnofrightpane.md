##PaneCollection.FirstVisibleColumnOfRightPane
PaneCollection property. Gets and sets the first visible column of the right pane
## PaneCollection.FirstVisibleColumnOfRightPane property
Gets and sets the first visible column of the right pane.
```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PaneCollectionPropertyFirstVisibleColumnOfRightPaneDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Freeze panes by specifying row and column indices (5, 3)
sheet.FreezePanes(5, 3, 5, 3);
// Get the panes collection
PaneCollection panes = sheet.GetPanes();
// Set the first visible column of the right pane
panes.FirstVisibleColumnOfRightPane = 1;
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
