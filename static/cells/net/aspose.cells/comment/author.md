##Comment.Author
Comment property. Gets and sets Name of the original comment author
## Comment.Author property
Gets and sets Name of the original comment author
```csharp
public string Author { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyAuthorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
// Set the comment author and note
comment.Author = "Carl.Yang";
comment.Note = "This is a sample comment";
// Display the comment author
Console.WriteLine("Comment Author: " + comment.Author);
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
