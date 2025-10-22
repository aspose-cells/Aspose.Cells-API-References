##RevisionInsertDelete.Revisions
RevisionInsertDelete property. Gets revision list by this operation
## RevisionInsertDelete.Revisions property
Gets revision list by this operation.
```csharp
public RevisionCollection Revisions { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionInsertDeletePropertyRevisionsDemo
{
public static void Run()
{
// Create a new workbook and enable revision tracking
Workbook workbook = new Workbook();
workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Perform operations to generate revisions
worksheet.Cells.InsertRows(0, 1);
worksheet.Cells.DeleteRows(1, 1);
// Get the revision logs
RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
// Iterate through all revision logs
foreach (RevisionLog revisionLog in revisionLogs)
{
foreach (Revision revision in revisionLog.Revisions)
{
if (revision is RevisionInsertDelete)
{
RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;
// Access the Revisions property (read-only)
RevisionCollection revisions = revisionInsertDelete.Revisions;
// Display information about the revisions
Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);
Console.WriteLine("Action Type: " + revisionInsertDelete.ActionType);
Console.WriteLine("Cell Area: " + revisionInsertDelete.CellArea);
Console.WriteLine("Number of related revisions: " + revisions.Count);
// Demonstrate usage of the Revisions collection
foreach (Revision relatedRevision in revisions)
{
Console.WriteLine(" - Related revision ID: " + relatedRevision.Id);
if (relatedRevision is RevisionInsertDelete)
{
RevisionInsertDelete relatedInsertDelete = (RevisionInsertDelete)relatedRevision;
Console.WriteLine("   Action Type: " + relatedInsertDelete.ActionType);
Console.WriteLine("   Cell Area: " + relatedInsertDelete.CellArea);
}
}
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionInsertDeletePropertyRevisionsDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCollection](../../revisioncollection/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
