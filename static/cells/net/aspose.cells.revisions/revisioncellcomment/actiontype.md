##RevisionCellComment.ActionType
RevisionCellComment property. Gets the action type of the revision
## RevisionCellComment.ActionType property
Gets the action type of the revision.
```csharp
public RevisionActionType ActionType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellCommentPropertyActionTypeDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
Comment comment = worksheet.Comments[0, 0];
comment.Note = "Initial comment";
// Modify the comment to generate a revision
comment.Note = "Updated comment";
// Add a new comment to generate an Add revision
Comment newComment = worksheet.Comments[1, 1];
newComment.Note = "New comment";
// Access the revisions
RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
foreach (Revision revision in revisions)
{
if (revision is RevisionCellComment)
{
RevisionCellComment commentRevision = (RevisionCellComment)revision;
// Display the ActionType property value
Console.WriteLine("Revision ActionType: " + commentRevision.ActionType);
// Demonstrate usage of ActionType property
switch (commentRevision.ActionType)
{
case RevisionActionType.Add:
Console.WriteLine("This revision added a new comment at " + commentRevision.CellName);
break;
case RevisionActionType.Delete:
Console.WriteLine("This revision deleted a comment from " + commentRevision.CellName);
break;
default:
Console.WriteLine("This revision modified a comment at " + commentRevision.CellName);
break;
}
// Show related properties
Console.WriteLine("Comment location: " + commentRevision.CellName);
Console.WriteLine("Is old comment: " + commentRevision.IsOldComment);
Console.WriteLine("Old length: " + commentRevision.OldLength);
Console.WriteLine("New length: " + commentRevision.NewLength);
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellCommentPropertyActionTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
