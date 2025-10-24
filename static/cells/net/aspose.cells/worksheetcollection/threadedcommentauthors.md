##WorksheetCollection.ThreadedCommentAuthors
WorksheetCollection property. Gets the list of threaded comment authors
## WorksheetCollection.ThreadedCommentAuthors property
Gets the list of threaded comment authors.
```csharp
public ThreadedCommentAuthorCollection ThreadedCommentAuthors { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyThreadedCommentAuthorsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a threaded comment author
int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demo", "DA");
// Get the author we just added
ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
// Add threaded comments to cell C2
AddThreadedComment(worksheet, "C2", "First comment", author);
AddThreadedComment(worksheet, "C2", "Second comment", author);
AddThreadedComment(worksheet, "C2", "Third comment", author);
// Save the workbook
workbook.Save("ThreadedCommentsDemo.xlsx");
}
private static void AddThreadedComment(Worksheet worksheet, string cellName, string text, ThreadedCommentAuthor author)
{
// Get the cell where we want to add the comment
Cell cell = worksheet.Cells[cellName];
// Add a threaded comment (returns void, not ThreadedComment)
worksheet.Comments.AddThreadedComment(cellName, text, author);
}
}
}
```
### See Also
* class [ThreadedCommentAuthorCollection](../../threadedcommentauthorcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
