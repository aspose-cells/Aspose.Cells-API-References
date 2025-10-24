##RevisionLog.Revisions
RevisionLog property. Gets all revisions in this log
## RevisionLog.Revisions property
Gets all revisions in this log.
```csharp
public RevisionCollection Revisions { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;
namespace AsposeCellsExamples
{
public class RevisionLogPropertyRevisionsDemo
{
public static void Run()
{
// Create a workbook with revision history
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Make some changes to track revisions
worksheet.Cells["A1"].PutValue("Initial Value");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].Formula = "=A2*2";
// Save with revision tracking
workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
// Make more changes to create revisions
worksheet.Cells["A1"].PutValue("Modified Value");
worksheet.Cells["A2"].PutValue(200);
// Save again to record revisions
workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
// Load the workbook with revisions
Workbook workbookWithRevisions = new Workbook("revision_demo.xlsx");
// Access revision logs
RevisionLogCollection revisionLogs = workbookWithRevisions.Worksheets.RevisionLogs;
// Process each revision log
foreach (RevisionLog log in revisionLogs)
{
Console.WriteLine($"Processing revision log with {log.Revisions.Count} revisions");
// Access revisions collection
RevisionCollection revisions = log.Revisions;
foreach (Revision revision in revisions)
{
Console.WriteLine($"Revision Type: {revision.Type}");
if (revision.Type == RevisionType.ChangeCells)
{
RevisionCellChange cellChange = (RevisionCellChange)revision;
Console.WriteLine($"Cell {cellChange.CellName} changed from '{cellChange.OldValue}' to '{cellChange.NewValue}'");
}
}
}
}
}
}
```
### See Also
* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
