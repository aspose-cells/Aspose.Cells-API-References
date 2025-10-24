##ThreadedComment.Row
ThreadedComment property. Gets the row index of the comment
## ThreadedComment.Row property
Gets the row index of the comment.
```csharp
public int Row { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ThreadedCommentPropertyRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create a threaded comment author
ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
author.Name = "Test Author";
author.UserId = "test@example.com";
// Add a threaded comment to cell B2 (row 1, column 1)
worksheet.Comments.AddThreadedComment(1, 1, "Sample threaded comment", author);
// Get the first threaded comment
ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
// Display the Row property value (read-only)
Console.WriteLine("Threaded comment row index: " + comment.Row);
// Verify the row index matches where we placed the comment
if (comment.Row == 1)
{
Console.WriteLine("Comment is correctly placed in row 1");
}
// Save the workbook
workbook.Save("ThreadedCommentRowDemo.xlsx");
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
