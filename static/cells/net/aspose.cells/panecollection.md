##Class PaneCollection
Aspose.Cells.PaneCollection class. Represents all Pane objects shown in the specified window
## PaneCollection class
Represents all Pane objects shown in the specified window.
```csharp
public class PaneCollection
```
## Properties
| Name | Description |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | Gets and sets the active pane. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | Gets and sets the first visible column of the right pane. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | Gets and sets the first visible row of the bottom pane. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassPaneCollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
sheet.Cells[i, j].Value = $"Row {i}, Col {j}";
}
}
// Freeze panes at row 5, column 1
sheet.FreezePanes(5, 1, 5, 1);
// Get pane collection
PaneCollection panes = sheet.GetPanes();
// Modify pane settings
panes.FirstVisibleRowOfBottomPane = 5;
panes.FirstVisibleColumnOfRightPane = 1;
// Save the workbook
workbook.Save("PaneCollectionDemo.xls", SaveFormat.Excel97To2003);
Console.WriteLine("PaneCollection demo executed successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
