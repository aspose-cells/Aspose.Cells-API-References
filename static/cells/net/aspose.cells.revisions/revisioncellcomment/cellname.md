##RevisionCellComment.CellName
RevisionCellComment property. Gets the name of the cell
## RevisionCellComment.CellName property
Gets the name of the cell.
```csharp
public string CellName { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;
public class RevisionCellCommentPropertyCellNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell B5
int commentRow = 4;
int commentCol = 1;
Comment comment = worksheet.Comments[commentRow, commentCol];
comment.Note = "Initial comment";
// Modify the comment to generate a revision
comment.Note = "Updated comment";
// Access the revisions
RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
foreach (Revision revision in revisions)
{
if (revision is RevisionCellComment)
{
RevisionCellComment commentRevision = (RevisionCellComment)revision;
// Display current CellName value
Console.WriteLine("Original CellName: " + commentRevision.CellName);
// Change the CellName property
commentRevision.CellName = "C10";
Console.WriteLine("Modified CellName: " + commentRevision.CellName);
// Demonstrate the effect of changing CellName
Console.WriteLine("Row index: " + commentRevision.Row);
Console.WriteLine("Column index: " + commentRevision.Column);
// Note: Changing CellName updates the Row/Column properties
Console.WriteLine("After CellName change - Row: " + commentRevision.Row);
Console.WriteLine("After CellName change - Column: " + commentRevision.Column);
}
}
// Save the workbook with revisions
workbook.Save("RevisionCellCommentPropertyCellNameDemo.xlsx");
}
}
}
```
### See Also
* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)
