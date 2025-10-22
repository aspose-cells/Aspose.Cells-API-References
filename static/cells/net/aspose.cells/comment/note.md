##Comment.Note
Comment property. Represents the content of comment
## Comment.Note property
Represents the content of comment.
```csharp
public string Note { get; set; }
```
### Remarks
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentPropertyNoteDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment1 = worksheet.Comments[commentIndex];
// Set the note for the comment
comment1.Note = "First note.";
// Verify the note was set
Console.WriteLine("Comment note: " + comment1.Note);
}
}
}
```
### See Also
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
