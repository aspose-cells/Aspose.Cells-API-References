##RevisionInsertDelete.Type
RevisionInsertDelete property. Represents the type of revision
## RevisionInsertDelete.Type property
Represents the type of revision.
```csharp
public override RevisionType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionInsertDeletePropertyTypeDemo
{
public static void Run()
{
// Create a new workbook and enable tracking revisions
Workbook workbook = new Workbook();
workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30; // Enable revision tracking by setting days
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Insert a row to generate a revision record
worksheet.Cells.InsertRows(0, 1);
// Get the revision collection (RevisionLogCollection itself is the collection)
RevisionLogCollection revisions = workbook.Worksheets.RevisionLogs;
// Find the RevisionInsertDelete in the revisions
foreach (RevisionLog revisionLog in revisions)
{
foreach (Revision revision in revisionLog.Revisions)
{
if (revision is RevisionInsertDelete)
{
RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;
// Display the Type property value
Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);
// Demonstrate usage of the Type property
if (revisionInsertDelete.Type == RevisionType.InsertDelete)
{
Console.WriteLine("This revision represents an insert/delete operation");
Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
Console.WriteLine("Action type: " + revisionInsertDelete.ActionType);
}
break;
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionInsertDeletePropertyTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
