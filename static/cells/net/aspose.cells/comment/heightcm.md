##Comment.HeightCM
Comment property. Represents the height of the comment in unit of centimeters
## Comment.HeightCM property
Represents the height of the comment, in unit of centimeters.
```csharp
public double HeightCM { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyHeightCMDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
// Set comment text
comment.Note = "Sample comment";
// Set comment height in centimeters
comment.HeightCM = 1.5;
// Save the workbook
workbook.Save("CommentHeightCMDemo.xlsx");
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
