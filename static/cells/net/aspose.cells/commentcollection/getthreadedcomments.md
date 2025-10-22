##CommentCollection.GetThreadedComments
CommentCollection method. Gets the threaded comments by row and column index
## GetThreadedComments(int, int) {#getthreadedcomments}
Gets the threaded comments by row and column index.
```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
### Examples
```csharp
[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
ThreadedComment tc = threadedComments1[i];
string note = tc.Notes;
}
```
### See Also
* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetThreadedComments(string) {#getthreadedcomments_1}
Gets the threaded comments by cell name.
```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CommentCollectionMethodGetThreadedCommentsWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a threaded comment author and get the author by index
int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "1");
ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
// Add a threaded comment to cell B2
worksheet.Comments.AddThreadedComment("B2", "Initial comment", author);
// Get all threaded comments for cell B2
ThreadedCommentCollection threadedComments = worksheet.Comments.GetThreadedComments("B2");
// Display the threaded comments
foreach (ThreadedComment comment in threadedComments)
{
Console.WriteLine($"Comment by {comment.Author.Name}: {comment.Notes}");
}
}
}
}
```
### See Also
* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
