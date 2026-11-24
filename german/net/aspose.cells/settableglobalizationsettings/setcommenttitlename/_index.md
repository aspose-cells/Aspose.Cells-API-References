---
title: "SettableGlobalizationSettings.SetCommentTitleName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SettableGlobalizationSettings-Methode. Gibt den lokalisierungsabhängigen Kommentar‑Titelnamen gemäß Kommentar‑Titeltyp zurück"
type: docs
url: /de/net/aspose.cells/settableglobalizationsettings/setcommenttitlename/
---
## SettableGlobalizationSettings.SetCommentTitleName method

Gibt den lokalisierungsabhängigen Kommentar‑Titelnamen gemäß dem Kommentar‑Titeltyp zurück.

```csharp
public void SetCommentTitleName(CommentTitleType type, string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | CommentTitleType | Typ des Kommentar‑Titels |
| Name | String | lokalisierungsabhängiger Kommentar‑Titelname |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodSetCommentTitleNameWithCommentTitleTypeStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einen Kommentar zur Zelle A1 hinzufügen
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            comment.IsVisible = true;

            // Erstellen Sie Globalisierungseinstellungen
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Legen Sie benutzerdefinierte Kommentar‑Titelnamen für verschiedene Typen fest
                settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Wenden Sie die Globalisierungseinstellungen auf die Arbeitsmappe an
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetCommentTitleName method executed successfully with parameters (CommentTitleType, String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCommentTitleName method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("MethodSetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


