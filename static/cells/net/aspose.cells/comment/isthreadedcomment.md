##Comment.IsThreadedComment
Comment property. Indicates whether this comment is a threaded comment
## Comment.IsThreadedComment property
Indicates whether this comment is a threaded comment.
```csharp
public bool IsThreadedComment { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyIsThreadedCommentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a regular comment
Comment regularComment = worksheet.Comments[worksheet.Comments.Add("A1")];
regularComment.Note = "This is a regular comment";
regularComment.Author = "User1";
// Add a threaded comment (assuming the API supports adding threaded comments)
Comment threadedComment = worksheet.Comments[worksheet.Comments.Add("B1")];
threadedComment.Note = "This is a threaded comment";
threadedComment.Author = "User2";
// Check comment types
Console.WriteLine("Comment at A1 is threaded: " + regularComment.IsThreadedComment);
Console.WriteLine("Comment at B1 is threaded: " + threadedComment.IsThreadedComment);
// Process comments based on their type
foreach (Comment comment in worksheet.Comments)
{
if (comment.IsThreadedComment)
{
Console.WriteLine($"Threaded comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
Console.WriteLine($"Author: {comment.Author}, Note: {comment.Note}");
}
else
{
Console.WriteLine($"Regular comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
}
}
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
