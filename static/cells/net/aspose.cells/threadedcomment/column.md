##ThreadedComment.Column
ThreadedComment property. Gets the column index of the comment
## ThreadedComment.Column property
Gets the column index of the comment.
```csharp
public int Column { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ThreadedCommentPropertyColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create a threaded comment author first
ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
// Add a threaded comment to cell A1 (row 0, column 0)
int commentRow = 0;
int commentColumn = 0;
worksheet.Comments.AddThreadedComment(commentRow, commentColumn, "Sample comment text", author);
// Get the first threaded comment
ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
// Display the Column property value (read-only)
Console.WriteLine("Threaded comment column index: " + comment.Column);
// Verify the column index matches where we placed the comment
if (comment.Column == commentColumn)
{
Console.WriteLine("Comment is correctly placed in column " + commentColumn);
}
// Save the workbook
workbook.Save("ThreadedCommentColumnDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
