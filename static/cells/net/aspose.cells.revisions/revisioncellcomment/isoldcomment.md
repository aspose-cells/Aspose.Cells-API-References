##RevisionCellComment.IsOldComment
RevisionCellComment property. Indicates whether its an old comment
## RevisionCellComment.IsOldComment property
Indicates whether it's an old comment.
```csharp
public bool IsOldComment { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellCommentPropertyIsOldCommentDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add initial comment to cell A1
Comment comment = worksheet.Comments[0, 0];
comment.Note = "First version of comment";
// Modify the comment to generate a revision
comment.Note = "Updated comment text";
// Add another comment to cell B2
Comment secondComment = worksheet.Comments[1, 1];
secondComment.Note = "Second comment";
// Access the revisions
RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
foreach (Revision revision in revisions)
{
if (revision is RevisionCellComment)
{
RevisionCellComment commentRevision = (RevisionCellComment)revision;
// Display IsOldComment property value
Console.WriteLine("Cell: " + commentRevision.CellName);
Console.WriteLine("IsOldComment: " + commentRevision.IsOldComment);
// Demonstrate usage of IsOldComment property
if (commentRevision.IsOldComment)
{
Console.WriteLine("This revision represents the old state of the comment");
Console.WriteLine("Old comment length: " + commentRevision.OldLength);
}
else
{
Console.WriteLine("This revision represents the new state of the comment");
Console.WriteLine("New comment length: " + commentRevision.NewLength);
}
// Show related properties
Console.WriteLine("Action Type: " + commentRevision.ActionType);
Console.WriteLine("Revision Type: " + commentRevision.Type);
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellCommentPropertyIsOldCommentDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
