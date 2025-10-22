##Comment.TextVerticalAlignment
Comment property. Gets and sets the text vertical alignment type of the comment
## Comment.TextVerticalAlignment property
Gets and sets the text vertical alignment type of the comment.
```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyTextVerticalAlignmentDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int commentIndex = worksheet.Comments.Add("B3");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "Sample comment text";
// Set vertical alignment to Fill
comment.TextVerticalAlignment = TextAlignmentType.Fill;
Console.WriteLine("Vertical Alignment: " + comment.TextVerticalAlignment);
// Change vertical alignment to Center if it was Fill
if (comment.TextVerticalAlignment == TextAlignmentType.Fill)
{
comment.TextVerticalAlignment = TextAlignmentType.Center;
Console.WriteLine("Changed Vertical Alignment to: " + comment.TextVerticalAlignment);
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
