##RevisionCellComment.Row
RevisionCellComment property. Gets the row index of the which contains a comment
## RevisionCellComment.Row property
Gets the row index of the which contains a comment.
```csharp
public int Row { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellCommentPropertyRowDemo
{
public static void Run()
{
// Create a new workbook with revision tracking
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell D4 (row 3, column 3)
int commentRow = 3;
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
// Display the Row property value
Console.WriteLine("Comment is located at row: " + commentRevision.Row);
// Demonstrate usage of Row property
Console.WriteLine("Comment location details:");
Console.WriteLine("Row index: " + commentRevision.Row);
Console.WriteLine("Column index: " + commentRevision.Column);
Console.WriteLine("Cell name: " + commentRevision.CellName);
// Show that Row is read-only by attempting to modify it (will cause compile error)
// commentRevision.Row = 5; // This line is commented out as Row is read-only
// Alternative way to change position by modifying CellName
Console.WriteLine("\nChanging comment position via CellName...");
commentRevision.CellName = "F10"; // Changes to row 9, column 5
Console.WriteLine("New Row index: " + commentRevision.Row);
Console.WriteLine("New Column index: " + commentRevision.Column);
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellCommentPropertyRowDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
