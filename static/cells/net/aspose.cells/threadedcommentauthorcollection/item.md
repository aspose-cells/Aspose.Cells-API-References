##ThreadedCommentAuthorCollection.Item
ThreadedCommentAuthorCollection property. Gets the person who create threaded comments
## ThreadedCommentAuthorCollection indexer (1 of 2)
Gets the person who create threaded comments.
```csharp
public ThreadedCommentAuthor this[int index] { get; }
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
public class ThreadedCommentAuthorCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
// Add authors and demonstrate Item property usage
authors.Add("John Doe", "john.doe@example.com", "JD");
authors.Add("Jane Smith", "jane.smith@example.com", "JS");
// Access author using Item property
ThreadedCommentAuthor firstAuthor = authors[0];
Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
// Set current person using Item property
authors.CurrentPerson = authors[1];
Console.WriteLine($"Current person: {authors.CurrentPerson.Name}");
// Add threaded comments
CommentCollection comments = workbook.Worksheets[0].Comments;
comments.AddThreadedComment("A1", "Comment from " + authors[0].Name, authors[0]);
comments.AddThreadedComment("A1", "Reply from " + authors[1].Name, authors[1]);
workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
}
}
}
```
### See Also
* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ThreadedCommentAuthorCollection indexer (2 of 2)
Gets the person who create threaded comments.
```csharp
public ThreadedCommentAuthor this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The name of the author. |
### See Also
* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
