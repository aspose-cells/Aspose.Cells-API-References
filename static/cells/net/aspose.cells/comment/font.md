##Comment.Font
Comment property. Gets the font of comment
## Comment.Font property
Gets the font of comment.
```csharp
public Font Font { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "Sample comment";
// Access and modify the font properties of the comment
Aspose.Cells.Font font = comment.Font;
font.Size = 12;
font.Name = "Arial";
font.Color = System.Drawing.Color.Red;
font.IsBold = true;
// Save the workbook
workbook.Save("CommentFontDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../../font/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
