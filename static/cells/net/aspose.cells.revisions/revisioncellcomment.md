##Class RevisionCellComment
Aspose.Cells.Revisions.RevisionCellComment class. Represents a revision record of a cell comment change
## RevisionCellComment class
Represents a revision record of a cell comment change.
```csharp
public class RevisionCellComment : Revision
```
## Properties
| Name | Description |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncellcomment/actiontype/) { get; } | Gets the action type of the revision. |
| [CellName](../../aspose.cells.revisions/revisioncellcomment/cellname/) { get; set; } | Gets the name of the cell. |
| [Column](../../aspose.cells.revisions/revisioncellcomment/column/) { get; } | Gets the column index of the which contains a comment. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| [IsOldComment](../../aspose.cells.revisions/revisioncellcomment/isoldcomment/) { get; } | Indicates whether it's an old comment. |
| [NewLength](../../aspose.cells.revisions/revisioncellcomment/newlength/) { get; } | Gets Length of the comment before this revision was made. |
| [OldLength](../../aspose.cells.revisions/revisioncellcomment/oldlength/) { get; } | Gets Length of the comment text added in this revision. |
| [Row](../../aspose.cells.revisions/revisioncellcomment/row/) { get; } | Gets the row index of the which contains a comment. |
| override [Type](../../aspose.cells.revisions/revisioncellcomment/type/) { get; } | Gets the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionsClassRevisionCellCommentDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add initial comment to cell A1
Comment comment = worksheet.Comments[0, 0];
comment.Note = "Initial comment text";
// Modify the comment to generate a revision
comment.Note = "Updated comment with more text";
// Access the revision log
RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
foreach (Revision revision in revisions)
{
if (revision is RevisionCellComment)
{
RevisionCellComment commentRevision = (RevisionCellComment)revision;
// Display revision properties
Console.WriteLine("Revision Type: " + commentRevision.Type);
Console.WriteLine("Action Type: " + commentRevision.ActionType);
Console.WriteLine("Cell Location: " + commentRevision.CellName);
Console.WriteLine("Row: " + commentRevision.Row);
Console.WriteLine("Column: " + commentRevision.Column);
// Show comment length changes
Console.WriteLine("Old Length: " + commentRevision.OldLength);
Console.WriteLine("New Length: " + commentRevision.NewLength);
Console.WriteLine("Is Old Comment: " + commentRevision.IsOldComment);
// Modify cell name to demonstrate property change
string originalCellName = commentRevision.CellName;
commentRevision.CellName = "B2";
Console.WriteLine("Modified Cell Location: " + commentRevision.CellName);
Console.WriteLine("New Row: " + commentRevision.Row);
Console.WriteLine("New Column: " + commentRevision.Column);
// Restore original cell name
commentRevision.CellName = originalCellName;
}
}
// Save the workbook with revisions
workbook.Save("RevisionsClassRevisionCellCommentDemo.xlsx");
}
}
}
```
### See Also
* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)
