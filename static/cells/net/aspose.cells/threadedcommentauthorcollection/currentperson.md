##ThreadedCommentAuthorCollection.CurrentPerson
ThreadedCommentAuthorCollection property. Gets and sets the current user
## ThreadedCommentAuthorCollection.CurrentPerson property
Gets and sets the current user.
```csharp
public ThreadedCommentAuthor CurrentPerson { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThreadedCommentAuthorCollectionPropertyCurrentPersonDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
int authorIndex = authors.Add("Jane Smith", "jane.smith@example.com", "provider456");
ThreadedCommentAuthor author = authors[authorIndex];
authors.CurrentPerson = author;
Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);
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
