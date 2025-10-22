##Comment.WidthCM
Comment property. Represents the width of the comment in unit of centimeters
## Comment.WidthCM property
Represents the width of the comment, in unit of centimeters.
```csharp
public double WidthCM { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyWidthCMDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "Sample comment";
comment.WidthCM = 5.0;
Console.WriteLine($"Comment width set to: {comment.WidthCM} cm");
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
