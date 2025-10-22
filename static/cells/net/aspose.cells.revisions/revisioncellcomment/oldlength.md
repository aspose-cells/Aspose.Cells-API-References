##RevisionCellComment.OldLength
RevisionCellComment property. Gets Length of the comment text added in this revision
## RevisionCellComment.OldLength property
Gets Length of the comment text added in this revision.
```csharp
public int OldLength { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellCommentPropertyOldLengthDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell D4
int commentRow = 3;
int commentCol = 3;
Comment comment = worksheet.Comments[commentRow, commentCol];
string initialComment = "Original comment text";
comment.Note = initialComment;
// Modify the comment to generate a revision
string updatedComment = "This is the modified comment text with more content";
comment.Note = updatedComment;
// Access the revisions
RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
foreach (Revision revision in revisions)
{
if (revision is RevisionCellComment)
{
RevisionCellComment commentRevision = (RevisionCellComment)revision;
// Display the OldLength property value
Console.WriteLine("Old comment length: " + commentRevision.OldLength);
Console.WriteLine("Actual initial comment length: " + initialComment.Length);
// Display related properties
Console.WriteLine("New comment length: " + commentRevision.NewLength);
Console.WriteLine("Comment location: " + commentRevision.CellName);
// Demonstrate usage of OldLength property
if (commentRevision.OldLength > 0)
{
Console.WriteLine("Comment existed before modification with length: " +
commentRevision.OldLength);
double expansionPercentage = ((double)(commentRevision.NewLength - commentRevision.OldLength) /
commentRevision.OldLength) * 100;
Console.WriteLine($"Comment expanded by {expansionPercentage:F2}%");
}
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellCommentPropertyOldLengthDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
