---
title: Enum CommentTitleType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.CommentTitleType enum. Represents comment title type while rendering when comment is set to display at end of sheet
type: docs
url: /net/aspose.cells.rendering/commenttitletype/
---
## CommentTitleType enumeration

Represents comment title type while rendering when comment is set to display at end of sheet.

```csharp
public enum CommentTitleType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Cell | `0` | Represents comment title cell. |
| Comment | `1` | Represents comment title comment. |
| Note | `2` | Represents comment title note. |
| Reply | `3` | Represents comment title reply. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create custom globalization settings
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

                // Demonstrate all CommentTitleType enum values
                Console.WriteLine("Available CommentTitleType values:");
                Console.WriteLine($"Cell: {(int)CommentTitleType.Cell}");
                Console.WriteLine($"Comment: {(int)CommentTitleType.Comment}");
                Console.WriteLine($"Note: {(int)CommentTitleType.Note}");
                Console.WriteLine($"Reply: {(int)CommentTitleType.Reply}");

                // Set custom titles for each comment type
                globalizationSettings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Apply the globalization settings to the workbook
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Add a comment to demonstrate the functionality
                int commentIndex = worksheet.Comments.Add("A1");
                Comment comment = worksheet.Comments[commentIndex];
                comment.Note = "This is a test comment";
                comment.Author = "Test Author";

                // Save the workbook
                workbook.Save("CommentTitleTypeDemo.xlsx");

                Console.WriteLine("CommentTitleType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CommentTitleType demonstration: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


