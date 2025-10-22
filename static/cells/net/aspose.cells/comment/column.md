##Comment.Column
Comment property. Gets the column index of the comment
## Comment.Column property
Gets the column index of the comment.
```csharp
public int Column { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell B5 (column index 1)
int commentRow = 4;
int commentColumn = 1;
Comment comment = worksheet.Comments[worksheet.Comments.Add(commentRow, commentColumn)];
// Set comment text
comment.Note = "This is a sample comment";
// Demonstrate Column property usage
Console.WriteLine("Comment is in column: " + comment.Column);
// Verify the column index matches where we placed it
if (comment.Column == commentColumn)
{
Console.WriteLine("Column property correctly returns the comment's column index");
}
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
