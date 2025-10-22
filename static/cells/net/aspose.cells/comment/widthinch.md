##Comment.WidthInch
Comment property. Represents the width of the comment in unit of inches
## Comment.WidthInch property
Represents the width of the comment, in unit of inches.
```csharp
public double WidthInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyWidthInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "Sample comment";
comment.WidthInch = 1.5;
Console.WriteLine("Comment width set to: " + comment.WidthInch + " inches");
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
