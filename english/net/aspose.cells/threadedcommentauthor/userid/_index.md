---
title: ThreadedCommentAuthor.UserId
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentAuthor property. Gets and sets the id of the user
type: docs
url: /net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

Gets and sets the id of the user.

```csharp
public string UserId { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyUserIdDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a threaded comment author with name, userId, and providerId
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");

                // Get the ThreadedCommentAuthor object
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

                // Display the UserId value (read operation)
                Console.WriteLine("Author UserId: " + author.UserId);

                // Demonstrate setting a new UserId (write operation)
                author.UserId = "NEW_USER_ID";
                Console.WriteLine("Updated UserId: " + author.UserId);

                // Create a threaded comment using the author
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);

                // Save the workbook
                workbook.Save("UserIdDemo.xlsx");

                Console.WriteLine("UserId property demonstration completed successfully.");
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


