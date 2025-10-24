##RevisionCellComment.Column
RevisionCellComment property. Gets the column index of the which contains a comment
## RevisionCellComment.Column property
Gets the column index of the which contains a comment.
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
public class RevisionCellCommentPropertyColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell D3
int commentRow = 2;
int commentCol = 3;
Comment comment = worksheet.Comments[commentRow, commentCol];
comment.Note = "Sample comment for revision tracking";
// Modify the comment to generate a revision
comment.Note = "Updated comment text";
// Access the revisions
RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
foreach (Revision revision in revisions)
{
if (revision is RevisionCellComment)
{
RevisionCellComment commentRevision = (RevisionCellComment)revision;
// Display the Column property value
Console.WriteLine("Comment revision column index: " + commentRevision.Column);
// Demonstrate usage of the Column property
Console.WriteLine("Comment was modified in column: " + (char)('A' + commentRevision.Column));
// Show related properties
Console.WriteLine("Associated row: " + commentRevision.Row);
Console.WriteLine("Cell name: " + commentRevision.CellName);
// Note: Column is read-only, so we can't modify it directly
// We can change it indirectly by modifying the CellName
string originalCellName = commentRevision.CellName;
commentRevision.CellName = "E5"; // This will update both Row and Column properties
Console.WriteLine("After CellName change - New column: " + commentRevision.Column);
// Restore original value
commentRevision.CellName = originalCellName;
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellCommentPropertyColumnDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
