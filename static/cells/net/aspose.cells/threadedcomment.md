##Class ThreadedComment
Aspose.Cells.ThreadedComment class. Represents the threaded comment
## ThreadedComment class
Represents the threaded comment.
```csharp
public class ThreadedComment
```
## Properties
| Name | Description |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | Gets the author of the comment. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | Gets the column index of the comment. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | Gets and sets the created time of this threaded comment. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | Gets and sets the text of the comment. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | Gets the row index of the comment. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassThreadedCommentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add authors to workbook
int author1Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User1", "user1@example.com", "1");
int author2Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User2", "", "2");
// Get author references
ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[author1Id];
ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[author2Id];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
// Add threaded comment to the comment
int threadedCommentIndex = comment.ThreadedComments.Add("This is a threaded comment", author1);
ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
// Set additional properties
threadedComment.Notes = "Additional notes";
// Add a reply to the threaded comment
int replyIndex = comment.ThreadedComments.Add("This is a reply", author2);
ThreadedComment reply = comment.ThreadedComments[replyIndex];
// Save the workbook
workbook.Save("ThreadedCommentDemo.xlsx");
Console.WriteLine("Threaded comment demo completed.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
