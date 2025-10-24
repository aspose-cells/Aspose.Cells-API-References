##ThreadedComment.CreatedTime
ThreadedComment property. Gets and sets the created time of this threaded comment
## ThreadedComment.CreatedTime property
Gets and sets the created time of this threaded comment.
```csharp
public DateTime CreatedTime { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThreadedCommentPropertyCreatedTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a threaded comment author
ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
// Add a comment to cell A1
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
// Add a threaded comment
int threadedCommentIndex = comment.ThreadedComments.Add("Test comment", author);
ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
// Demonstrate CreatedTime property
Console.WriteLine("Threaded comment created at: " + threadedComment.CreatedTime);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
