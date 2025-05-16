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
namespace AsposeCellsExamples.RenderingClassCommentTitleTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;

    public class RenderingClassCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook and access first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample comment to cell A1
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "Important note for review";
            comment.Font.Size = 14;

            // Configure comments to display at end of sheet when rendering
            worksheet.PageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;

            // Create PDF save options and configure comment title type
            PdfSaveOptions options = new PdfSaveOptions();
            // Note: CommentTitleType property is not available in PdfSaveOptions as per the current API definitions

            // Save workbook with rendering configuration
            workbook.Save("CommentTitleTypeDemo.pdf", options);
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


