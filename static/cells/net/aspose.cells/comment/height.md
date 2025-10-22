##Comment.Height
Comment property. Represents the Height of the comment in unit of pixels
## Comment.Height property
Represents the Height of the comment, in unit of pixels.
```csharp
public int Height { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyHeightDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "Sample comment";
// Demonstrate Height property
comment.Height = 100;
Console.WriteLine("Comment height set to: " + comment.Height);
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
