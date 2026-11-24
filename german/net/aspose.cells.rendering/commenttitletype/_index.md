---
title: "Aufzählung CommentTitleType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.CommentTitleType Enum. Stellt den Kommentar‑Titeltyp beim Rendern dar, wenn der Kommentar am Ende des Blatts angezeigt wird."
type: docs
url: /de/net/aspose.cells.rendering/commenttitletype/
---
## CommentTitleType enumeration

Stellt den Kommentar‑Titeltyp beim Rendern dar, wenn der Kommentar am Ende des Arbeitsblatts angezeigt werden soll.

```csharp
public enum CommentTitleType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Cell | `0` | Stellt die Kommentar‑Titelzelle dar. |
| Comment | `1` | Stellt den Kommentar‑Titelkommentar dar. |
| Note | `2` | Stellt die Kommentar‑Titelnotiz dar. |
| Reply | `3` | Stellt die Kommentar‑Titelantwort dar. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle benutzerdefinierte Globalisierungseinstellungen
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

                // Demonstriere alle Werte der CommentTitleType‑Enum
                Console.WriteLine("Available CommentTitleType values:");
                Console.WriteLine($"Cell: {(int)CommentTitleType.Cell}");
                Console.WriteLine($"Comment: {(int)CommentTitleType.Comment}");
                Console.WriteLine($"Note: {(int)CommentTitleType.Note}");
                Console.WriteLine($"Reply: {(int)CommentTitleType.Reply}");

                // Setze benutzerdefinierte Titel für jeden Kommentar‑Typ
                globalizationSettings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Wenden Sie die Globalisierungseinstellungen auf die Arbeitsmappe an
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Füge einen Kommentar hinzu, um die Funktionalität zu demonstrieren
                int commentIndex = worksheet.Comments.Add("A1");
                Comment comment = worksheet.Comments[commentIndex];
                comment.Note = "This is a test comment";
                comment.Author = "Test Author";

                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


