##Enum PaneStateType
Aspose.Cells.PaneStateType enum. Represents state of the sheets pane
## PaneStateType enumeration
Represents state of the sheet's pane.
```csharp
public enum PaneStateType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Frozen | `0` | Panes are frozen, but were not before being frozen. |
| FrozenSplit | `1` | Panes are frozen and were split before being frozen. |
| Split | `2` | Panes are split, but not frozen. |
| Normal | `3` | Panes are not frozen and not split. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class PaneStateTypeDemo
{
public static void PaneStateTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Set some sample data in the worksheet
worksheet.Cells["A1"].PutValue("Data 1");
worksheet.Cells["A2"].PutValue("Data 2");
worksheet.Cells["A3"].PutValue("Data 3");
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
// Freeze panes at cell B2
worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column
// Check the pane state
PaneStateType paneState = worksheet.PaneState;
// Output the pane state
Console.WriteLine("Current Pane State: " + paneState);
// Save the workbook
workbook.Save("PaneStateTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
