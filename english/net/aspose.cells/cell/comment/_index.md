---
title: Cell.Comment
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the comment of this cell
type: docs
url: /net/aspose.cells/cell/comment/
---
## Cell.Comment property

Gets the comment of this cell.

```csharp
public Comment Comment { get; }
```

### Remarks

If there is no comment applies to the cell, returns null.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a comment to cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell");

            // Add a comment to the cell
            Comment comment = cell.Comment;
            if (comment == null)
            {
                // Create a new comment if none exists
                int commentIndex = worksheet.Comments.Add("A1");
                comment = worksheet.Comments[commentIndex];
                comment.Author = "Author Name";
                comment.Note = "This is a sample comment";
            }

            try
            {
                // Display the comment properties
                Console.WriteLine("Comment Author: " + comment.Author);
                Console.WriteLine("Comment Note: " + comment.Note);
                Console.WriteLine("Comment Row: " + comment.Row);
                Console.WriteLine("Comment Column: " + comment.Column);
                Console.WriteLine("Comment is Visible: " + comment.IsVisible);

                // Modify some comment properties
                comment.Note = "Updated comment text";
                comment.IsVisible = true;

                // Display updated comment note
                Console.WriteLine("Updated Comment Note: " + comment.Note);

                // Save the workbook
                workbook.Save("CommentDemo.xlsx");
                Console.WriteLine("Comment has been demonstrated and saved to CommentDemo.xlsx");
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

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


