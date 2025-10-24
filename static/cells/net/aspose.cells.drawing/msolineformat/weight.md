##MsoLineFormat.Weight
MsoLineFormat property. Returns or sets the weight of the line in units of pt
## MsoLineFormat.Weight property
Returns or sets the weight of the line ,in units of pt.
```csharp
public double Weight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MsoLineFormatPropertyWeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
// Set the comment text
comment.Note = "Sample comment";
// Access the comment shape's line format and set the weight
comment.CommentShape.LineFormat.Weight = 0.75;
// Save the workbook
workbook.Save("output.xlsx");
// Verify the weight was set correctly
Console.WriteLine("Line weight: " + worksheet.Comments[0].CommentShape.LineFormat.Weight);
}
}
}
```
### See Also
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
