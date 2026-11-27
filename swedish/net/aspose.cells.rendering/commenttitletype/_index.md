---
title: "Enum CommentTitleType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.CommentTitleType enum. Representerar kommentarsrubriktyp vid rendering när kommentaren är inställd på att visas i slutet av bladet"
type: docs
url: /sv/net/aspose.cells.rendering/commenttitletype/
---
## CommentTitleType enumeration

Representerar kommentarsrubriktyp vid rendering när kommentaren är inställd på att visas i slutet av bladet.

```csharp
public enum CommentTitleType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Cell | `0` | Representerar kommentarsrubrikcell. |
| Comment | `1` | Representerar kommentarsrubrikkommentar. |
| Note | `2` | Representerar kommentarsrubrikanteckning. |
| Reply | `3` | Representerar kommentarsrubriksvaret. |

### Exempel

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
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa anpassade globaliseringsinställningar
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

                // Demonstrera alla CommentTitleType enum‑värden
                Console.WriteLine("Available CommentTitleType values:");
                Console.WriteLine($"Cell: {(int)CommentTitleType.Cell}");
                Console.WriteLine($"Comment: {(int)CommentTitleType.Comment}");
                Console.WriteLine($"Note: {(int)CommentTitleType.Note}");
                Console.WriteLine($"Reply: {(int)CommentTitleType.Reply}");

                // Ange anpassade rubriker för varje kommentarstyp
                globalizationSettings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Applicera globaliseringsinställningarna på arbetsboken
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Lägg till en kommentar för att demonstrera funktionaliteten
                int commentIndex = worksheet.Comments.Add("A1");
                Comment comment = worksheet.Comments[commentIndex];
                comment.Note = "This is a test comment";
                comment.Author = "Test Author";

                // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


