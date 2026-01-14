---
title: ThreadedComment.Notes
second_title: Aspose.Cells for .NET API Reference
description: ThreadedComment property. Gets and sets the text of the comment
type: docs
url: /net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

Gets and sets the text of the comment.

```csharp
public string Notes { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyNotesDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create or obtain a threaded comment author
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
                author.Name = "User1";

                // Add a threaded comment to cell A1 (row 0, column 0) with initial text
                worksheet.Comments.AddThreadedComment(0, 0, "Initial comment text", author);

                // Retrieve the newly added threaded comment
                ThreadedComment threadedComment = worksheet.Comments[0].ThreadedComments[0];

                // Update the Notes property (the comment text)
                threadedComment.Notes = "Updated comment notes";

                // Read and display the Notes property value
                Console.WriteLine("Threaded comment Notes: " + threadedComment.Notes);

                // Save the workbook (optional)
                workbook.Save("ThreadedCommentNotesDemo.xlsx");
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

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


