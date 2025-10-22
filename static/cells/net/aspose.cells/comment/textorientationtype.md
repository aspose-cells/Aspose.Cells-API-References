##Comment.TextOrientationType
Comment property. Gets and sets the text orientation type of the comment
## Comment.TextOrientationType property
Gets and sets the text orientation type of the comment.
```csharp
public TextOrientationType TextOrientationType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyTextOrientationTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "Sample comment text";
// Set initial orientation to NoRotation
comment.TextOrientationType = TextOrientationType.NoRotation;
Console.WriteLine("Initial orientation: " + comment.TextOrientationType);
// Change orientation to TopToBottom if currently NoRotation
if (comment.TextOrientationType == TextOrientationType.NoRotation)
{
comment.TextOrientationType = TextOrientationType.TopToBottom;
Console.WriteLine("Changed orientation to: " + comment.TextOrientationType);
}
// Save the workbook
workbook.Save("CommentOrientationDemo.xlsx");
}
}
}
```
### See Also
* enum [TextOrientationType](../../textorientationtype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
