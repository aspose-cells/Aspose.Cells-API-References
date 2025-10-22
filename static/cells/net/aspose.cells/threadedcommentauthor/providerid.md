##ThreadedCommentAuthor.ProviderId
ThreadedCommentAuthor property. Gets the id of the provider
## ThreadedCommentAuthor.ProviderId property
Gets the id of the provider.
```csharp
public string ProviderId { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ThreadedCommentAuthorPropertyProviderIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Add a threaded comment author and get its index
int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");
// Get the ThreadedCommentAuthor object
ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
// Display the ProviderId value (read operation)
Console.WriteLine("Author ProviderId: " + author.ProviderId);
// Create a threaded comment using the author
worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);
// Save the workbook
workbook.Save("ThreadedCommentAuthorDemo.xlsx");
Console.WriteLine("Demo completed successfully.");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
