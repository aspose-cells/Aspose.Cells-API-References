##ThreadedCommentAuthorCollection.IndexOf
ThreadedCommentAuthorCollection method. Gets the index of ThreadedCommentAuthor object
## ThreadedCommentAuthorCollection.IndexOf method
Gets the index of ThreadedCommentAuthor object
```csharp
public int IndexOf(ThreadedCommentAuthor author)
```
| Parameter | Type | Description |
| --- | --- | --- |
| author | ThreadedCommentAuthor | The ThreadedCommentAuthor object |
### Return Value
The index in the ThreadedCommentAuthor collection
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ThreadedCommentAuthorCollectionMethodIndexOfWithThreadedCommentAuthorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the threaded comment authors collection
ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
// Add authors to the collection
int johnIndex = authors.Add("John Doe", "john.doe", "provider1");
int janeIndex = authors.Add("Jane Smith", "jane.smith", "provider2");
// Get the author objects
ThreadedCommentAuthor johnAuthor = authors[johnIndex];
ThreadedCommentAuthor janeAuthor = authors[janeIndex];
try
{
// Call IndexOf method to find the position of Jane Smith
int foundIndex = authors.IndexOf(janeAuthor);
// Display the result
Console.WriteLine($"Author '{janeAuthor.Name}' found at index: {foundIndex}");
// Verify the result matches the expected index
if (foundIndex == janeIndex)
{
Console.WriteLine("IndexOf result matches the expected index");
}
else
{
Console.WriteLine("IndexOf result does not match the expected index");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
}
// Save the workbook
workbook.Save("ThreadedCommentAuthorIndexOfDemo.xlsx");
}
}
}
```
### See Also
* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
