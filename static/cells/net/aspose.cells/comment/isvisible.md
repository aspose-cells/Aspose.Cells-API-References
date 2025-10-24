##Comment.IsVisible
Comment property. Represents if the comment is visible or not
## Comment.IsVisible property
Represents if the comment is visible or not.
```csharp
public bool IsVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyIsVisibleDemo
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
// Set the comment to be visible
comment.IsVisible = true;
// Check if the comment is visible
if (comment.IsVisible)
{
Console.WriteLine("The comment is visible");
}
// Save the workbook
workbook.Save("CommentVisibilityDemo.xlsx");
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
