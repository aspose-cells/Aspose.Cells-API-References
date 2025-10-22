##ThreadedCommentCollection.Item
ThreadedCommentCollection property. Gets the threaded comment by the specific index
## ThreadedCommentCollection indexer
Gets the threaded comment by the specific index.
```csharp
public ThreadedComment this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThreadedCommentCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment
Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
comment.Note = "Initial comment";
// Add threaded comments
ThreadedCommentCollection threadedComments = comment.ThreadedComments;
ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
// Add authors
int author1Index = authors.Add("User1", "user1@example.com", "ID1");
int author2Index = authors.Add("User2", "user2@example.com", "ID2");
// Add threaded comments
threadedComments.Add("Reply 1", authors[author1Index]);
threadedComments.Add("Reply 2", authors[author2Index]);
// Demonstrate Item property usage
ThreadedComment firstComment = threadedComments[0];
ThreadedComment secondComment = threadedComments[1];
Console.WriteLine("First comment author: " + firstComment.Author.Name);
Console.WriteLine("Second comment author: " + secondComment.Author.Name);
// Modify second comment's author
secondComment.Author = authors[author1Index];
Console.WriteLine("Updated second comment author: " + secondComment.Author.Name);
// Save the workbook
workbook.Save("ThreadedCommentsDemo.xlsx");
}
}
}
```
### See Also
* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
