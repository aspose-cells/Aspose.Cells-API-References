##MsoFillFormat.Transparency
MsoFillFormat property. Returns or sets the degree of transparency of the specified fill as a value from 0.0 opaque through 1.0 clear
## MsoFillFormat.Transparency property
Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoFillFormatPropertyTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "This is a test comment";
// Set fill format properties including transparency
comment.CommentShape.FillFormat.IsVisible = true;
comment.CommentShape.FillFormat.ForeColor = System.Drawing.Color.Red;
comment.CommentShape.FillFormat.BackColor = System.Drawing.Color.Yellow;
// Set transparency (0.0 = fully opaque, 1.0 = fully transparent)
comment.CommentShape.FillFormat.Transparency = 0.5;
// Save the workbook
workbook.Save("CommentTransparencyDemo.xlsx");
// Load the saved workbook to verify transparency
Workbook verifyWorkbook = new Workbook("CommentTransparencyDemo.xlsx");
Comment verifyComment = verifyWorkbook.Worksheets[0].Comments[0];
// Output the transparency value to demonstrate it was saved and loaded correctly
Console.WriteLine("Comment fill transparency: " +
verifyComment.CommentShape.FillFormat.Transparency);
}
}
}
```
### See Also
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
