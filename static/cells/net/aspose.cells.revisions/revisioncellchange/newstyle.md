##RevisionCellChange.NewStyle
RevisionCellChange property. Gets the new style of the cell
## RevisionCellChange.NewStyle property
Gets the new style of the cell.
```csharp
public Style NewStyle { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellChangePropertyNewStyleDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
// No direct StartTrackingRevisions method available - revisions are tracked automatically
Worksheet worksheet = workbook.Worksheets[0];
// Modify a cell to generate a revision
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Original Value");
Style originalStyle = workbook.CreateStyle();
originalStyle.Font.Name = "Arial";
originalStyle.Font.Size = 10;
cell.SetStyle(originalStyle);
// Change the cell to create a revision
cell.PutValue("New Value");
Style newStyle = workbook.CreateStyle();
newStyle.Font.Name = "Times New Roman";
newStyle.Font.Size = 12;
newStyle.Font.IsBold = true;
cell.SetStyle(newStyle);
// No direct StopTrackingRevisions method available
// Access the revision log through RevisionLogs instead of Revisions
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
foreach (RevisionLog log in revisionLogs)
{
foreach (Revision revision in log.Revisions)
{
if (revision is RevisionCellChange cellChange)
{
// Display information about the cell change revision
Console.WriteLine("Cell Name: " + cellChange.CellName);
Console.WriteLine("Old Value: " + cellChange.OldValue);
Console.WriteLine("New Value: " + cellChange.NewValue);
// Access the NewStyle property
Style revisionNewStyle = cellChange.NewStyle;
Console.WriteLine("\nNew Style Properties:");
Console.WriteLine("Font Name: " + revisionNewStyle.Font.Name);
Console.WriteLine("Font Size: " + revisionNewStyle.Font.Size);
Console.WriteLine("Is Bold: " + revisionNewStyle.Font.IsBold);
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellChangePropertyNewStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
