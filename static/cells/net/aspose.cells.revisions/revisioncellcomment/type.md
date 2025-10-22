##RevisionCellComment.Type
RevisionCellComment property. Gets the type of revision
## RevisionCellComment.Type property
Gets the type of revision.
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
public class RevisionCellCommentPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentRow = 0;
int commentCol = 0;
Comment comment = worksheet.Comments[commentRow, commentCol];
comment.Note = "Initial comment";
// Track revisions - changed to use HasRevisions property
// Note: In actual usage, you might need to enable tracking through other means
// as HasRevisions is a read-only property that indicates if revisions exist
// Modify the comment to generate a revision
comment.Note = "Modified comment";
// Access the revisions through the Workbook's RevisionLogs collection
RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
foreach (Revision revision in revisions)
{
if (revision is RevisionCellComment)
{
RevisionCellComment commentRevision = (RevisionCellComment)revision;
// Display the Type property value
Console.WriteLine("Revision Type: " + commentRevision.Type);
// Demonstrate usage of the Type property
if (commentRevision.Type == RevisionType.Comment)
{
Console.WriteLine("This revision is related to a comment change");
Console.WriteLine("Comment was modified at row: " + commentRevision.Row + ", column: " + commentRevision.Column);
Console.WriteLine("Old comment length: " + commentRevision.OldLength);
Console.WriteLine("New comment length: " + commentRevision.NewLength);
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellCommentPropertyTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [RevisionType](../../revisiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
