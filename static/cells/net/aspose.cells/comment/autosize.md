##Comment.AutoSize
Comment property. Indicates if size of comment is adjusted automatically according to its content. Note In some special cases such as Mac environment this setting may not take effect. If this setting does not take effect please replace it with FitToTextSize
## Comment.AutoSize property
Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize().
```csharp
public bool AutoSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyAutoSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "This is a sample comment that will auto-size to fit its content.";
// Set AutoSize to true
comment.AutoSize = true;
// Save the workbook
workbook.Save("CommentAutoSizeDemo.xlsx");
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
