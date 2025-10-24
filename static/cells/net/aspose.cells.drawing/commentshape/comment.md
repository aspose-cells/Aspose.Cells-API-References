##CommentShape.Comment
CommentShape property. Gets the comment object
## CommentShape.Comment property
Gets the comment object.
```csharp
public Comment Comment { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class CommentShapePropertyCommentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "This is a sample comment";
// Get the comment shape and demonstrate Comment property
CommentShape commentShape = worksheet.Comments[commentIndex].CommentShape;
Comment retrievedComment = commentShape.Comment;
// Display the comment text
Console.WriteLine("Comment Text: " + retrievedComment.Note);
}
}
}
```
### See Also
* class [Comment](../../../aspose.cells/comment/)
* class [CommentShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
