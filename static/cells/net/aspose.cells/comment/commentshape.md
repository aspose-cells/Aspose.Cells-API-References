##Comment.CommentShape
Comment property. Get a Shape object that represents the shape attached to the specified comment
## Comment.CommentShape property
Get a Shape object that represents the shape attached to the specified comment.
```csharp
public CommentShape CommentShape { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class CommentPropertyCommentShapeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment1 = worksheet.Comments[commentIndex];
comment1.Note = "This is a sample comment";
// Get the CommentShape and modify its properties
Shape shape = comment1.CommentShape;
shape.Width = 200;
shape.Height = 100;
shape.FillFormat.ForeColor = System.Drawing.Color.LightYellow;
shape.LineFormat.ForeColor = System.Drawing.Color.Blue;
// Display the shape dimensions
Console.WriteLine("Comment shape width: " + shape.Width);
Console.WriteLine("Comment shape height: " + shape.Height);
}
}
}
```
### See Also
* class [CommentShape](../../../aspose.cells.drawing/commentshape/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
