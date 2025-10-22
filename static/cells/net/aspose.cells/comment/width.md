##Comment.Width
Comment property. Represents the width of the comment in unit of pixels
## Comment.Width property
Represents the width of the comment, in unit of pixels.
```csharp
public int Width { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyWidthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
// Set comment properties
comment.Note = "This is a sample comment";
comment.Width = 200; // Setting the width of the comment box
comment.Height = 50;
// Save the workbook
workbook.Save("CommentWidthDemo.xlsx");
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
