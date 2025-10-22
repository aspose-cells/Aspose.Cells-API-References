##RevisionCellChange.Column
RevisionCellChange property. Gets the column index of the cell
## RevisionCellChange.Column property
Gets the column index of the cell.
```csharp
public int Column { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellChangePropertyColumnDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Modify cell B2 to generate a revision
Cell cell = worksheet.Cells["B2"];
cell.PutValue("Initial Value");
// Change the cell to create a revision
cell.PutValue("Modified Value");
// Access the revision logs
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
foreach (RevisionLog log in revisionLogs)
{
foreach (Revision revision in log.Revisions)
{
if (revision is RevisionCellChange cellChange)
{
// Display column information from the revision
Console.WriteLine("Cell Name: " + cellChange.CellName);
Console.WriteLine("Column Index: " + cellChange.Column);
Console.WriteLine("Row Index: " + cellChange.Row);
// Demonstrate using the Column property
if (cellChange.Column == 1) // Column B is index 1
{
Console.WriteLine("\nThis revision affects column B");
Console.WriteLine("Old Value: " + cellChange.OldValue);
Console.WriteLine("New Value: " + cellChange.NewValue);
}
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellChangePropertyColumnDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
