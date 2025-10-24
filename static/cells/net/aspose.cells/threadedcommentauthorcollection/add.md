##ThreadedCommentAuthorCollection.Add
ThreadedCommentAuthorCollection method. Adds one thread comment person
## ThreadedCommentAuthorCollection.Add method
Adds one thread comment person.
```csharp
public int Add(string name, string userId, string providerId)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the person. |
| userId | String |  |
| providerId | String | The id of the provider |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThreadedCommentAuthorCollectionMethodAddWithStringStringStringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a threaded comment author
int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Test Author", "testuser", "TA");
// Get the added author
ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
// Add threaded comments using the author
worksheet.Comments.AddThreadedComment("C2", "First comment", author);
worksheet.Comments.AddThreadedComment("C2", "Second comment", author);
// Save the workbook
workbook.Save("ThreadedCommentsExample.xlsx");
}
}
}
```
### See Also
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
