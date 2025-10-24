##ThreadedCommentAuthor.Name
ThreadedCommentAuthor property. Gets and sets the name
## ThreadedCommentAuthor.Name property
Gets and sets the name.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThreadedCommentAuthorPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a comment and threaded comments
int commentIndex = worksheet.Comments.Add("A1");
Comment comment = worksheet.Comments[commentIndex];
comment.Note = "Initial comment";
ThreadedCommentCollection threadedComments = comment.ThreadedComments;
// Add threaded comments with different authors
ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
int author1Index = authors.Add("User1", "user1@example.com", "ID1");
int author2Index = authors.Add("User2", "user2@example.com", "ID2");
// Add threaded comments
threadedComments.Add("Reply from User1", authors[author1Index]);
threadedComments.Add("Reply from User2", authors[author2Index]);
// Demonstrate Name property usage
Console.WriteLine("First author name: " + threadedComments[0].Author.Name);
Console.WriteLine("Second author name: " + threadedComments[1].Author.Name);
// Change author of second comment
threadedComments[1].Author = authors[author1Index];
Console.WriteLine("Updated second author name: " + threadedComments[1].Author.Name);
// Save the workbook
workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
}
}
}
```
### See Also
* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
