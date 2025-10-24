##Worksheet.PaneState
Worksheet property. Indicates whether the pane has horizontal or vertical splits and whether those splits are frozen
## Worksheet.PaneState property
Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen.
```csharp
public PaneStateType PaneState { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyPaneStateDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Item 1");
worksheet.Cells["A3"].PutValue("Item 2");
// Freeze panes (first row)
worksheet.FreezePanes(1, 0, 1, 0);
// Get and display pane state
PaneStateType paneState = worksheet.PaneState;
Console.WriteLine("Pane State: " + paneState);
// Save workbook
workbook.Save("PaneStateDemo.xlsx");
}
}
}
```
### See Also
* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
