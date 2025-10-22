##Comment.TextHorizontalAlignment
Comment property. Gets and sets the text horizontal alignment type of the comment
## Comment.TextHorizontalAlignment property
Gets and sets the text horizontal alignment type of the comment.
```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyTextHorizontalAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "Sample comment text";
// Set initial horizontal alignment to Fill
comment.TextHorizontalAlignment = TextAlignmentType.Fill;
Console.WriteLine("Initial alignment: " + comment.TextHorizontalAlignment);
// Change alignment to Center if it was Fill
if (comment.TextHorizontalAlignment == TextAlignmentType.Fill)
{
comment.TextHorizontalAlignment = TextAlignmentType.Center;
Console.WriteLine("Updated alignment: " + comment.TextHorizontalAlignment);
}
}
}
}
```
### See Also
* enum [TextAlignmentType](../../textalignmenttype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
