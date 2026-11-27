---
title: "GlobalizationSettings.GetCommentTitleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metod. Hämtar det lokalberoende kommentarsrubriknamnet enligt kommentarsrubriktyp"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getcommenttitlename/
---
## GlobalizationSettings.GetCommentTitleName method

Hämtar det lokalanpassade kommentarsrubriknamnet enligt kommentarsrubriktyp.

```csharp
public virtual string GetCommentTitleName(CommentTitleType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | CommentTitleType |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo : GlobalizationSettings
    {
        public override string GetCommentTitleName(CommentTitleType type)
        {
            switch (type)
            {
                case CommentTitleType.Cell:
                    return "Custom Cell Comment";
                case CommentTitleType.Reply:  // Changed from Threaded to Reply
                    return "Custom Threaded Comment";
                default:
                    return base.GetCommentTitleName(type);
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new GlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo(); // Changed to use Settings

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till testkommentar
            int commentIndex = worksheet.Comments.Add("B5");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Test comment content";

            try
            {
                // Hämta kommentarsrubrik för olika typer
                var cellTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Cell); // Changed to use Settings
                var threadedTitle = workbook.Settings.GlobalizationSettings.GetCommentTitleName(CommentTitleType.Reply); // Changed type and Settings

                Console.WriteLine($"Cell Comment Title: {cellTitle}");
                Console.WriteLine($"Threaded Comment Title: {threadedTitle}");

                // Ange kommentarförfattare (rubrik) med våra anpassade globalization-inställningar
                comment.Author = cellTitle; // Changed from Title to Author
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            workbook.Save("GetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


