##Comment.Row
Comment property. Gets the row index of the comment
## Comment.Row property
Gets the row index of the comment.
```csharp
public int Row { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment1 = worksheet.Comments[commentIndex];
comment1.Note = "This is a sample comment";
// Get and display the row index of the commented cell
int row = comment1.Row;
Console.WriteLine("The comment is in row: " + row);
// Add another comment to cell B3
commentIndex = worksheet.Comments.Add("B3");
Comment comment2 = worksheet.Comments[commentIndex];
comment2.Note = "Another comment";
// Display row index of second comment
Console.WriteLine("Second comment is in row: " + comment2.Row);
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
