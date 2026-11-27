---
title: "SettableGlobalizationSettings.GetCommentTitleName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Hämtar det lokalanpassade kommentarsrubriknamnet enligt kommentarsrubriktyp"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/getcommenttitlename/
---
## SettableGlobalizationSettings.GetCommentTitleName method

Hämtar det lokalanpassade kommentarsrubriknamnet enligt kommentarsrubriktyp.

```csharp
public override string GetCommentTitleName(CommentTitleType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | CommentTitleType | typ av kommentarsrubrik |

### Returvärde

lokalanpassat kommentarsrubriknamn

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodGetCommentTitleNameWithCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en kommentar i cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            comment.IsVisible = true;

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Ange anpassade kommentarsrubriknamn för olika typer
            settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
            settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
            settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
            settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

            // Applicera globaliseringsinställningarna på arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Hämta och visa kommentarsrubriknamnen
                Console.WriteLine("Cell title: " + settings.GetCommentTitleName(CommentTitleType.Cell));
                Console.WriteLine("Comment title: " + settings.GetCommentTitleName(CommentTitleType.Comment));
                Console.WriteLine("Note title: " + settings.GetCommentTitleName(CommentTitleType.Note));
                Console.WriteLine("Reply title: " + settings.GetCommentTitleName(CommentTitleType.Reply));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCommentTitleName method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("CommentTitleNamesDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


