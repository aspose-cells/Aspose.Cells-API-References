---
title: "SettableGlobalizationSettings.SetCommentTitleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Hämtar det lokalanpassade kommentarsrubriknamnet enligt kommentarsrubriktyp"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setcommenttitlename/
---
## SettableGlobalizationSettings.SetCommentTitleName method

Hämtar det lokalanpassade kommentarsrubriknamnet enligt kommentarsrubriktyp.

```csharp
public void SetCommentTitleName(CommentTitleType type, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | CommentTitleType | typ av kommentarsrubrik |
| namn | String | lokalanpassat kommentarsrubriknamn |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            comment.IsVisible = true;

            // Skapa globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Ange anpassade kommentarsrubriknamn för olika typer
                settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Applicera globaliseringsinställningarna på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetCommentTitleName method executed successfully with parameters (CommentTitleType, String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCommentTitleName method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("MethodSetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


