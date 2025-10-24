##RevisionCellComment.NewLength
RevisionCellComment property. Gets Length of the comment before this revision was made
## RevisionCellComment.NewLength property
Gets Length of the comment before this revision was made.
```csharp
public int NewLength { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellCommentPropertyNewLengthDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell F7
int commentRow = 6;
int commentCol = 5;
Comment comment = worksheet.Comments[commentRow, commentCol];
comment.Note = "Initial comment text";
// Modify the comment to generate a revision
string updatedComment = "This is an updated and longer comment text";
comment.Note = updatedComment;
// Access the revisions
RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
foreach (Revision revision in revisions)
{
if (revision is RevisionCellComment)
{
RevisionCellComment commentRevision = (RevisionCellComment)revision;
// Display the NewLength property value
Console.WriteLine("New comment length: " + commentRevision.NewLength);
Console.WriteLine("Actual new comment length: " + updatedComment.Length);
// Display related properties
Console.WriteLine("Old comment length: " + commentRevision.OldLength);
Console.WriteLine("Comment location: " + commentRevision.CellName);
// Demonstrate usage of NewLength property
if (commentRevision.NewLength > commentRevision.OldLength)
{
Console.WriteLine("Comment was expanded by " +
(commentRevision.NewLength - commentRevision.OldLength) + " characters");
}
else if (commentRevision.NewLength < commentRevision.OldLength)
{
Console.WriteLine("Comment was shortened by " +
(commentRevision.OldLength - commentRevision.NewLength) + " characters");
}
else
{
Console.WriteLine("Comment length remained the same");
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellCommentPropertyNewLengthDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
