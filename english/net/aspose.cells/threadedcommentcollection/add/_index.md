---
title: ThreadedCommentCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentCollection method. Adds a threaded comment
type: docs
url: /net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Adds a threaded comment.

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of the threaded comment. |
| author | ThreadedCommentAuthor | The author of the threaded comment |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentCollectionMethodAddWithStringThreadedCommentDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for context
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Create a threaded comment author using the ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
                int authorIndex = authors.Add("John Doe", "john.doe@example.com", "EXAMPLE_PROVIDER");
                ThreadedCommentAuthor author = authors[authorIndex];

                // Access the threaded comments collection of a cell
                Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
                ThreadedCommentCollection threadedComments = comment.ThreadedComments;

                // Call the Add method with String and ThreadedCommentAuthor parameters
                int commentIndex = threadedComments.Add("This is a threaded comment", author);

                // Display the result
                Console.WriteLine($"Added threaded comment at index: {commentIndex}");
                Console.WriteLine($"Comment text: {threadedComments[commentIndex].Notes}");
                Console.WriteLine($"Author: {threadedComments[commentIndex].Author.Name}");

                // Save the workbook
                workbook.Save("ThreadedCommentAddDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


