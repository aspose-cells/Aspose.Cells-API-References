---
title: ThreadedComment.Author
second_title: Aspose.Cells for .NET API Reference
description: ThreadedComment property. Gets the author of the comment
type: docs
url: /net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

Gets the author of the comment.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Get the default threaded comment author from the workbook
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "John Doe";
                author.UserId = "john.doe@example.com";

                // Add a threaded comment to cell A1 (row 0, column 0)
                worksheet.Comments.AddThreadedComment(0, 0, "Sample comment", author);

                // Get the first threaded comment
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];

                // Display the Author property value (read operation)
                Console.WriteLine("Author Name: " + comment.Author.Name);
                Console.WriteLine("Author UserId: " + comment.Author.UserId);
                Console.WriteLine("Author ProviderId: " + comment.Author.ProviderId);

                // Demonstrate setting the Author property (since it's read/write)
                ThreadedCommentAuthor newAuthor = workbook.Worksheets.ThreadedCommentAuthors[0];
                newAuthor.Name = "Jane Smith";
                newAuthor.UserId = "jane.smith@example.com";
                comment.Author = newAuthor;

                // Display the updated Author property value
                Console.WriteLine("Updated Author Name: " + comment.Author.Name);
                Console.WriteLine("Updated Author UserId: " + comment.Author.UserId);

                // Save the workbook
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
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
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


