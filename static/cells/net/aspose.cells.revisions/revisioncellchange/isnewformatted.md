##RevisionCellChange.IsNewFormatted
RevisionCellChange property. Indicates whether this cell is new formatted
## RevisionCellChange.IsNewFormatted property
Indicates whether this cell is new formatted.
```csharp
public bool IsNewFormatted { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellChangePropertyIsNewFormattedDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set initial cell value and style
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Initial Value");
Style initialStyle = workbook.CreateStyle();
initialStyle.Font.Name = "Arial";
initialStyle.Font.Size = 10;
cell.SetStyle(initialStyle);
// Change the cell value and style to create a revision
cell.PutValue("Updated Value");
Style newStyle = workbook.CreateStyle();
newStyle.Font.Name = "Calibri";
newStyle.Font.Size = 12;
newStyle.Font.IsBold = true;
cell.SetStyle(newStyle);
// Access the revision logs
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
foreach (RevisionLog log in revisionLogs)
{
foreach (Revision revision in log.Revisions)
{
if (revision is RevisionCellChange cellChange)
{
// Display revision information
Console.WriteLine("Cell Name: " + cellChange.CellName);
Console.WriteLine("Old Value: " + cellChange.OldValue);
Console.WriteLine("New Value: " + cellChange.NewValue);
// Demonstrate IsNewFormatted property
Console.WriteLine("\nFormatting Information:");
Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);
Console.WriteLine("IsNewFormatted: " + cellChange.IsNewFormatted);
if (cellChange.IsNewFormatted)
{
Console.WriteLine("The cell has new formatting applied in this revision.");
Console.WriteLine("New Font: " + cellChange.NewStyle.Font.Name);
Console.WriteLine("New Font Size: " + cellChange.NewStyle.Font.Size);
Console.WriteLine("Is Bold: " + cellChange.NewStyle.Font.IsBold);
}
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellChangePropertyIsNewFormattedDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
